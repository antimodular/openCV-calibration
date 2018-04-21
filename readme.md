## Information
This is an on-going collection of openCV camera calibration files for variouse cameras that are used for camera intrinsic parameters calibration and image undistortion.

## Notes
I am using the calibration example that comes with the [ofxCv](https://github.com/kylemcdonald/ofxCv/tree/master/example-calibration) addon for openframeworks.
To make it work with wide angle lenses i needed to make this change in calibration.cpp:
```
//        int calibFlags = 0;
int calibFlags =CV_CALIB_FIX_PRINCIPAL_POINT | CV_CALIB_ZERO_TANGENT_DIST | CV_CALIB_FIX_FOCAL_LENGTH | CV_CALIB_FIX_ASPECT_RATIO | CV_CALIB_FIX_K3 | CV_CALIB_FIX_K4 | CV_CALIB_FIX_K5 | CV_CALIB_FIX_K6;
```

## Links
https://forum.openframeworks.cc/t/ofxcv-calibration-artifacts/23614

https://forum.openframeworks.cc/t/calibrate-fisheye-lens-ofxcv/20600
