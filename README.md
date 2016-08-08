# pangolin_android
a repository for pangolin on android

## MainPage
this repository is aimed at transplanting pangolin to android.The Author of Pangolin is stevenlovegrove and source repository is:[https://github.com/stevenlovegrove/Pangolin](https://github.com/stevenlovegrove/Pangolin).Introduction about pangolin detail can be found at source code's github page. Original Pangolin contains a method to transplant it to android however hard to achieve with some errors inside the CMakeLists and source code.I made a small change for Pangolin to make it suitable for OPENGL ES/ES2.

## Code
Find the latest version on [Github](https://github.com):
``` 
 git clone https://github.com/FangGet/pangolin_android.git
```

## Standalone Libs And Examples
compiled libs and examples for android can be found here: [http://pan.baidu.com/s/1c2dXRXm](http://pan.baidu.com/s/1c2dXRXm);

## Dependencies
* Android SDK;
* Android NDK(>R5E);
* Android-Cmake(given);

you should have installed Android SDK in your Linux and environment variables should have been setted properly. SDK have to be updated with version>android-8.

Android NDK can be only extracted in certain directory.

Android-Cmake may not perform properly on Windows.

Other dependencies for pangolin can be found at[https://github.com/FangGet/pangolin_android/tree/master/Pangolin](https://github.com/FangGet/pangolin_android/tree/master/Pangolin).

## Building
pangolin_android uses CMake portable pre-build tool. Please excute the following at a shell (or the equivelent using a GUI):
```
git clone  https://github.com/FangGet/pangolin_android.git
export $ANDROID_NDK=you android ndk root directory
cd pangolin_android
mkdir build
cd build
cmake -DCMAKE_TOOLCHAIN_FILE=android.toolchain.cmake \
      -DANDROID_NDK=<ndk_path>                       \
      -DCMAKE_BUILD_TYPE=Release                     \
      -DANDROID_ABI="armeabi-v7a with NEON"          \
      -DANDROID_NATIVE_API_LEVEL=android-14
      <source_path>
 cmake --build 
```

## Issues
Please visit [Github Issues](https://github.com/FangGet/pangolin_android/issues) to view and report problems with Pangolin. I will try my best to answer it.

Contact with: fangasfrank@gmail.com
