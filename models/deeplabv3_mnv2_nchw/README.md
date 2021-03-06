`.npy` files under this folder are downloaded from ONNX model of DeepLab V3 MoblieNet V2 generated by following commands, which is licensed under the Apache 2.0.

### How to Generate DeepLab V3 MobileNet V2 ONNX model

Following this [guide](../deeplabv3_mnv2_nhwc#how-to-generate-deeplab-v3-mobilenet-v2-tflite-model) to generate the DeepLab V3 MoblieNet V2 TFLite model, then use ['tf2onnx'](https://github.com/onnx/tensorflow-onnx) tool to convert TFLite model to ONNX model:

```
python3 -m tf2onnx.convert --opset 13 --tflite deeplab_mobilenetv2.tflite --output deeplab_mobilenetv2.onnx
```