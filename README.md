# task
1. All container should be created in same network
> we created same network "mynetwork" with bridge.

2. Application container data should be persisted
> we created volume for that like
volumes:
  db-data:
  wordpress-data:


3. Configurable fields should be passed as Environment variables
> we created .env file and mention the version of apps


4. Automatically restart if the container fails
> we set policy for that
restart: always

5. configure minimum CPU and memory limits for containers
>we set limit for CPU and memory
deploy:
      resources:
        limits:
          cpus: '0.5'
          memory: 50M
6. Choose light weighted image
>we use alpine version of some image but not working proper because it doesnt have that binary

7. Vulnerabilities in the image should be less
> we created strong application security



![Screenshot (171)](https://user-images.githubusercontent.com/94424237/165456143-ad0b73ad-8861-4dae-bc41-469dbc22dd0c.png)

using alpine image 

![Screenshot (172)](https://user-images.githubusercontent.com/94424237/165456257-01f7d391-3ff6-4222-87f2-e89e8eca6d97.png)
