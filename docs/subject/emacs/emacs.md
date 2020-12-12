## 编译emacs
```
./autogen.sh
mkdir build
cd build
../configure --prefix=/mnt/hdd1/tools/emacs --with-xml2 --with-json --with-xpm --with-jpeg --with-tiff --with-gif --with-png --with-rsvg --without-gnutls
make -sj
make install
```
### 需要的包
```
sudo apt install texinfo
sudo apt install libxml2-dev
sudo apt install libjpeg-dev
sudo apt install libgif-dev
sudo apt install libtiff-dev

```

不建议安装，可以通过配置选项关闭gnutls

```sudo apt install libgnutls28-dev```

## Emacs PPA添加
```
sudo add-apt-repository -y ppa:ubuntu-elisp
sudo apt-get update
sudo apt-get install emacs-snapshot
```
https://launchpad.net/~ubuntu-elisp/+archive/ubuntu/ppa
