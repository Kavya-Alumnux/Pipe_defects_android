## Info
This branch provides tflite based pipe defects detection for android. 
There are 5 classes which will be detected: cracks, debris, joint displacement, broken and roots.


## Usage

### 1. Put TFLite model in `assets` folder of Android project, and change 
- `inputSize` to `--img`
- `output_width` according to new/old `inputSize` ratio
- `anchors` to `m.anchor_grid` as https://github.com/ultralytics/yolov5/pull/1127#issuecomment-714651073
in android/app/src/main/java/org/tensorflow/lite/examples/detection/tflite/DetectorFactory.java
### 2. Put labels.txt file in 'assets' folder as well.

Then run the program in Android Studio.

