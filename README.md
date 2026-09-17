# Hello CMake
## 项目简介

使用 CMake 构建的 C++ 程序，运行后输出 `Hello, RoboMaster!`

## 环境
- Ubuntu 22.04.5 LTS
- CMake 3.22.1
- GCC 11.4.0
安装命令：
sudo apt update
sudo apt upgrade -y
sudo apt install -y build-essential cmake git
验证：
lsb_release -a
g++ --version
cmake --version
git --version


## 目录结构
hello_cmake/
├── CMakeLists.txt   # 构建规则
├── README.md        # 说明文档
├── .gitignore       # Git 忽略清单
├── src/             # 源代码目录，存放编写的源代码，与其他目录区分开
│   └── main.cpp
├── images/          # 存放截图，展示程序确实是在Ubuntu上构建并运行，展示可信度
│   └── success.png
└── build/           # CMake 自动生成的构建目录，存放编译中间文件和可执行文件
## 构建步骤
```bash
cmake -S . -B build
cmake --build build
./build/hello

## 运行结果

```bash
./build/hello
```
输出：

```
Hello, RoboMaster!
```
运行成功截图：
![运行成功截图](images/success.png)


## 作者和日期

盛明伟 2253211152  完成日期：2026年9月17日
