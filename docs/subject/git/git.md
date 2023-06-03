## git clone加速代理
```git config --global url."https://ghproxy.com/".insteadOf https://```
## git关闭SSL校验设置
```git config --global http.sslVerify false```
## git设置默认编辑器为VIM
```git config --global core.editor "vim"```
## git 设置和取消代理
```
git config --global http.proxy http://username:password@127.0.0.1:1080
git config --global https.proxy https://username:password@127.0.0.1:1080
```
```
git config --global --unset http.proxy
git config --global --unset https.proxy
```
## 编译git with openssl
```
./configure --prefix=/mnt/hdd1/tools/git --with-openssl=YES --with-curl=YES --with-expat=YES
make all doc -sj
```
### 需要的包：
```
-lexpat: sudo apt install libexpat1-dev
-lcurl: sudo apt install libcurl4-openssl-dev
sudo apt install gettext
sudo apt install asciidoc
```
