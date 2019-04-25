Steps
=========
1. Clone the repository
2. Make sure that `docker` and `docker-compose` are installed, you can check it by the command `docker --version` and `docker-compose --version`
2. `sudo docker-compose up`
3. Make sure that ports 3306 and 8000 are not occupied(do `sudo service mysql stop`, to stop mysql which usually runs on 3306 port) 
3. Do `sudo docker ps` and copy the container id of rajchandvaniya/quantiphi_workshop
4.`sudo docker exec -it <copied_id> python3 /code/manage.py migrate`
5. Go to url http://localhost:8000
