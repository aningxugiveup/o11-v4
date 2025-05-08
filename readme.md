```bash


docker pull docker.io/library/ubuntu:22.04

git clone https://github.com/aningxugiveup/o11-v4

cd o11-v4

sudo docker build -t o11-v4 .

### Choose between nodejs or python. DONT FORGET TO ADD YOUR SERVER IP ADDRESS!!!

# nodejs (default) 
sudo docker run -d -p 18080:18080 -p 18443:18443 -p 15454:15454 -p 18484:18484 -e IP_ADDRESS=SERVER-IP-HERE -e SERVER_TYPE=nodejs --name o11 o11-v4

# python
sudo docker run -d -p 18080:18080 -p 18443:18443 -p 15454:15454 -p 18484:18484 -e IP_ADDRESS=SERVER-IP-HERE-e SERVER_TYPE=python --name o11 o11-v4

# Web Panel: http://SERVER-IP-HERE:18484
# Credentials: admin:admin

```
