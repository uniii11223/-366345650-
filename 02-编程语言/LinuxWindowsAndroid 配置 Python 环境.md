【问题】Linux/Windows/Android 配置 Python 环境常见问题
【环境】Linux(Ubuntu/CentOS)、Windows 10/11、Android (Termux)
【解决方案】
1. Linux (Ubuntu) 安装 Python 3.9+

· 更新源：sudo apt update
· 安装依赖：sudo apt install software-properties-common
· 添加 deadsnakes 源：sudo add-apt-repository ppa:deadsnakes/ppa
· 安装 Python：sudo apt install python3.9
· 验证：python3.9 --version

2. Linux (CentOS/RHEL) 编译安装 Python 3.9

· 安装编译依赖：sudo yum install gcc openssl-devel bzip2-devel libffi-devel -y
· 下载源码：wget https://www.python.org/ftp/python/3.9.0/Python-3.9.0.tgz
· 解压并进入目录：tar -xzf Python-3.9.0.tgz && cd Python-3.9.0
· 配置与编译：./configure --enable-optimizations && sudo make altinstall
· 验证：python3.9 --version

3. Windows 安装 Python 3.9

· 访问官网下载：https://www.python.org/downloads/
· 选择 Windows  installer (64位)
· 安装时务必勾选 “Add Python to PATH”
· 验证：打开 CMD，输入 python --version

4. Android (Termux) 安装 Python 3.9

· 更新源：pkg update && pkg upgrade
· 安装 Python：pkg install python
· 若需指定 Python 3.9 版本，可尝试：pkg install python@3.9
· 验证：python --version

【贡献者】@AM Tirster
【收录日期】2026.03.15
