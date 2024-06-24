# rPi-5-Install-PyCharm

I tried to install the Jet Brains toolbox, but I didn't succeed. I installed PyCharm without the toolbox.

## Install Pycharm without the toolbox

# Update the system
```
sudo apt-get update
sudo apt-get upgrade
```
# Install JAVA
```
sudo apt install openjdk-21-jdk openjdk-21-jre
```
# Check active JAVA version
```
sudo update-alternatives --display java

java - auto mode
  link best version is /usr/lib/jvm/java-21-openjdk-arm64/bin/java
  <pre>
  <b>link currently points to /usr/lib/jvm/java-21-openjdk-arm64/bin/java</b>
  </pre>
  link java is /usr/bin/java
  slave java.1.gz is /usr/share/man/man1/java.1.gz
/usr/lib/jvm/java-17-openjdk-arm64/bin/java - priority 1711
  slave java.1.gz: /usr/lib/jvm/java-17-openjdk-arm64/man/man1/java.1.gz
/usr/lib/jvm/java-21-openjdk-arm64/bin/java - priority 2111
  slave java.1.gz: /usr/lib/jvm/java-21-openjdk-arm64/man/man1/java.1.gz
```
```
sudo update-alternatives --config java
There are 2 choices for the alternative java (providing /usr/bin/java).

  Selection    Path                                         Priority   Status
------------------------------------------------------------
  0            /usr/lib/jvm/java-21-openjdk-arm64/bin/java   2111      auto mode
* 1            /usr/lib/jvm/java-17-openjdk-arm64/bin/java   1711      manual mode
  2            /usr/lib/jvm/java-21-openjdk-arm64/bin/java   2111      manual mode

```











## my try to install the Jet Brains toolbox

`sudo apt install libfuse2`

```
ownload the tarball .tar.gz from the Toolbox App web page.

https://www.jetbrains.com/toolbox-app/

.tar.gz (Linux ARM64)

extract to /opt/

sudo tar -xzf jetbrains-toolbox-2.3.2.31487-arm64.tar.gz -C /opt


cd jetbrains-toolbox-2.3.2.31487/

./jetbrains-toolbox

apt install openjdk-21-jdk openjdk-21-jre

sudo apt update
sudo apt install build-essential

sudo apt install gawk
sudo apt install bison



wget -c https://ftp.gnu.org/gnu/glibc/glibc-2.29.tar.gz

tar -zxvf glibc-2.29.tar.gz
mkdir glibc-2.29/build
cd glibc-2.29/build
../configure --prefix=/opt/glibc
make 
make install
```
