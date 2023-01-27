1) Launch a t2.micro instance in Mumbai region where ssh can be done only via your IP address with git, docker and docker-compose installed it using user-data script


login aws account and launch instance mubail regeion and add user data

#!/bin/bash

sudo yum install docker -y
sudo systemctl start docker
sudo systemctl enable docker
sudo curl -L https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
sudo yum install git -y



![Screenshot (382)](https://user-images.githubusercontent.com/119240540/215174275-cee2ac15-9f4a-453e-bb28-597099c1d212.png)


![Screenshot (384)](https://user-images.githubusercontent.com/119240540/215174203-f7ab7fa7-979c-4af9-baeb-ac059a8fb7f8.png)

and launch instance


check it 
![Screenshot (385)](https://user-images.githubusercontent.com/119240540/215174434-30b3dc59-bc4b-4219-857f-c2c29675ac9f.png)

Elastic IP addresses very time new instance we can user that ip 

![Screenshot (386)](https://user-images.githubusercontent.com/119240540/215174771-0fc4ffa2-feee-4af8-b563-39285ec2eda2.png)


![Screenshot (387)](https://user-images.githubusercontent.com/119240540/215174746-98a61154-0042-4d1d-a79d-1544ffe7c196.png)
![Screenshot (388)](https://user-images.githubusercontent.com/119240540/215174756-8ee0be6e-f302-47cc-aeb7-ce955f9fe239.png)
![Screenshot (389)](https://user-images.githubusercontent.com/119240540/215174765-5eb8f42e-f783-4ba9-900b-a295c4c5519e.png)
