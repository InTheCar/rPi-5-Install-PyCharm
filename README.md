# rPi-5-Install-PyCharm

nstall the Toolbox App
sudo apt install libfuse2


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



wget -c https://ftp.gnu.org/gnu/glibc/glibc-2.39.tar.gz
tar -zxvf glibc-2.39.tar.gz
mkdir glibc-2.39/build
cd glibc-2.39/build
../configure --prefix=/opt/glibc
make 
make install
