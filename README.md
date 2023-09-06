**Task 2: Microservices Architecture and Deployment**
1. Docker Should be Installed on your device. If it is not installed, first Install docker following this [link](https://docs.docker.com/get-docker/)
2. **Fork saleor-platfrom repository** to your GitHub by following this [link](https://github.com/saleor/saleor-platform) 
3. **Clone the forked Repo** to your device. As for me i used to following command git clone https://github.com/syedmohaiman/saleor-platform.git
4. **Go to the cloned directory:** cd saleor-platform
5. **Build the application**: docker compose build
6. **Apply Django migrations**: docker compose run --rm api python3 manage.py migrate
7. **Populate the database** with example data and create the admin user: docker compose run --rm api python3 manage.py populatedb --createsuperuser
8. **Run the application**:docker compose up
9. **Start the saleor-platform** Using the Following link to : http://localhost:9000/
 The application will start. 
![image](https://github.com/syedmohaiman/isec6000-assignment1-task2/assets/37250700/fc43328c-e616-4e9c-a7d5-544fd7439829)
10. **Change the port from 9000 to 9003** by modifying compose.yml file : nano docker-compose.yml
11. **Shut down the Docker**: docker compose down
12. **Start Docker**: docker compose up -d
13. **Start saleor-platform with new port 9003** Using the Following link to : http://localhost:9003/
 The application will start. 
![image](https://github.com/syedmohaiman/isec6000-assignment1-task2/assets/37250700/03cf7de6-9309-47a5-80d1-bad7189f73b5)
