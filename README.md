# my-laravel-app
If you haven't already created a Laravel application, create a new Laravel project named:

`my-laravel-app`- mkdir my-laravel-app
--------------------------------------------------
**Step 2: Create Dockerfile**
Create a `Dockerfile` in the root of your Laravel project

sudo vi Dockerfile
--------------------------------------------------
**Step 3: Create Docker Compose File**
Create a `docker-compose.yml` file in the root of your Laravel project 

sudo vi docker-compose.yml
---------------------------------------------------
**Step 4: Nginx Configuration**

Create a `docker/nginx.conf` file for Nginx configuration. This file should configure Nginx to serve your Laravel application:
---------------------------------------------------
**Step 5: Update Laravel Environment Configuration**

Update your `.env` file to match the database configuration defined in `docker-compose.yml`
----------------------------------------------------
**Step 6: Build and Run Docker Containers**
Now, you can build and start your Docker containers using Docker Compose:


docker-compose up --build  //  
docker-compose up -d
----------------------------------------------------
**7. Access Your Laravel Application**

Open your web browser and navigate to `http://localhost:8000`. You should see the Laravel welcome page.
----------------------------------------------------
**8. (Optional) Run Laravel Migrations**

docker-compose exec app php artisan migrate   //  
docker-compose exec app php artisan db:seed 
-----------------------------------------------------
