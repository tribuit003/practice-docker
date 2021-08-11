Cài đặt Server

Boot:1GB
SWAP:2GB
/:

root:1
ebui:x

ssh root@192.168.3.134 -A

curl -sSL https://get.docker.com | sudo -E sh
// wait 5mins

cd /etc/sudoers.d/
touch client
vi 
usermod -a -G sudo

systemctl enable docker
systemctl start docker
sudo usermod -aG docker ebui

yum update
// wait 10mins

vi /etc/yum.conf
exclude=centos-release*

https://docker-py.readthedocs.io/en/stable/

docker login

sudo yum install git

sudo yum install epel-release

sudo yum install python3-pip

pip install docker

yum install wget
wget https://bootstrap.pypa.io/pip/2.7/get-pip.py
python get-pip.py
yum install python3

admin/ebui

pip install virtualenv
virtualenv djangoenv
source djangoenv/bin/activate
pip install django
django-admin startproject prj1
---
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver 0.0.0.0:8000
---
deactivate

sudo pip3 install virtualenv
python3 -m virtualenv venv
source venv/bin/activate
sudo pip3 install Django==2.1.2
django-admin startproject project
---
sudo python3 manage.py migrate
sudo python3 manage.py createsuperuser
sudo python3 manage.py runserver 0.0.0.0:8000s
sudo python3 manage.py runserver 0.0.0.0:80
---
deactivate

yum install net-tools

sudo python3 manage.py startapp home
python3 manage.py runserver 0.0.0.0:80

sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

docker-compose up -d
(network)
(volume)

docker-compose down --volumes

pip3 install jinja2