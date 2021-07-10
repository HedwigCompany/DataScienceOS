# DataScienceOS
Datascience Development Environment 

- pip kurulumu:
```bash
sudo apt-get install python3-pip
```
- virtualenv kurulumu:
```bash
sudo pip3 install virtualenv
```
- python 2.7 kurulumu:
```bash
sudo apt install python
```
- python 3 kurulumu:
```bash
sudo apt install python3
```
- python2 virtualenv oluþturma ve aktive etme:
```bash
sudo virtualenv python2env
sudo virtualenv -p /usr/bin/python2.7 python2env
source python2env/bin/activate
```
- python3 virtualenv oluþturma ve aktive etme:
```bash
sudo virtualenv -p python3 python3env
source python3env/bin/activate
```
- python kütüphaneleri kurulum:
> ** Python 3
```bash
source python3env/bin/activate

pip3 install scipy
pip3 install scikit-learn
pip3 install numpy
pip3 install matplotlib
pip3 install pandas
pip3 install SymPy

deactivate
```
> ** Python 2
```bash
source python2env/bin/activate

pip install scipy
pip install scikit-learn
pip install numpy
pip install matplotlib
pip install pandas
pip install SymPy
```
- pyCharm kurulum:
```bash
sudo snap install pycharm-community --classic
```
- R Kurulum:
```bash
sudo apt -y install r-base
R kütüphanelerini arama:
apt search r-cran lib-ismi
**Örn:** apt search r-cran r-cran-gplots
```
- R Kütüphanelerini Kurma:
```bash
sudo apt install r-cran-gplots
sudo apt install r-cran-ggplot2
sudo apt install r-cran-dplyr
sudo apt install r-cran-lubridate
sudo apt install r-cran-zoo
```
- R Command Line ile Kurulan Library'ler:
```bash
install.packages("sqldf")
install.packages('forecast', dependencies = TRUE)
```
- R Studio Kurulum:
```bash
sudo apt install gdebi-core
wget https://download1.rstudio.org/rstudio-xenial-1.1.453-amd64.deb
sudo gdebi rstudio-xenial-1.1.453-amd64.deb
```
- Install Oracle Java:
```bash
sudo apt-add-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer
```
- HADOOP:
```bash
wget http://ftp.itu.edu.tr/Mirror/Apache/hadoop/common/hadoop-3.1.0/hadoop-3.1.0.tar.gz
sudo tar -xzvf hadoop-3.1.0.tar.gz -C /opt/
```
- SCALA:
```bash
sudo wget https://www.scala-lang.org/files/archive/scala-2.12.6.deb
sudo dpkg -i scala-2.12.6.deb
```
- SPARK:
```bash
wget http://ftp.itu.edu.tr/Mirror/Apache/spark/spark-2.3.0/spark-2.3.0-bin-hadoop2.7.tgz
sudo tar -xzvf spark-2.3.0-bin-hadoop2.7.tgz -C /opt
```
- ZOOKEEPER:
```bash
wget http://ftp.itu.edu.tr/Mirror/Apache/zookeeper/zookeeper-3.4.12/zookeeper-3.4.12.tar.gz
sudo tar -xzvf zookeeper-3.4.12.tar.gz -C /opt
```
- KAFKA:
```bash
wget http://ftp.itu.edu.tr/Mirror/Apache/kafka/1.1.0/kafka_2.12-1.1.0.tgz
sudo tar -xzvf kafka_2.12-1.1.0.tgz -C /opt
```
- TENSORFLOW:
```bash
mkdir ~/tensorflowenv
```
> ** Python 2 için:
```bash
virtualenv --system-site-packages tensorflowenv
```
> ** Python 3 için:
```bash
virtualenv --system-site-packages -p python3 tensorflowenv
source ~/tensorflowenv/bin/activate
pip install --upgrade tensorflow
```
