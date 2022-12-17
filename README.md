### 0x1 安装依赖
- brew install libusb  
- brew install libiconv

## 开始编译
需要替换下 CMakeLists.txt 里面 libusb 的版本号，比如我这里是是 1.0.25
```
set (libusb_INCLUDE_DIR "/usr/local/Cellar/libusb/1.0.25/include/libusb-1.0/")
set (libusb_STATIC "/usr/local/Cellar/libusb/1.0.25/lib/")
```
直接编译就好了
```
mkdir build
cd build
cmake ../
make
```
就能直接看到生成 rkDevelopTool_Mac

