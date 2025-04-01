```bash


docker pull docker.io/library/ubuntu:22.04

git clone https://github.com/pigzillaaaaa/o11-v4

cd o11-v4

sudo docker build -t o11-v4 .

### Choose between nodejs or python. DONT FORGET TO ADD YOUR SERVER IP ADDRESS!!!

# nodejs (default) 
sudo docker run -d -p 80:80 -p 443:443 -p 5454:5454 -p 8484:8484 -e IP_ADDRESS=SERVER-IP-HERE -e SERVER_TYPE=nodejs --name o11 o11-v4

# python
sudo docker run -d -p 80:80 -p 443:443 -p 5454:5454 -p 8484:8484 -e IP_ADDRESS=SERVER-IP-HERE-e SERVER_TYPE=python --name o11 o11-v4

# Web Panel: http://SERVER-IP-HERE:8484
# Credentials: admin:admin

```
