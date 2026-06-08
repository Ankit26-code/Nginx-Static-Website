# Nginx-Static-Website 
Using Dockerfile 

Create Index.html file 
then
Create Dockerfile

FROM nginx
COPY . /usr/share/nginx/html
EXPOSE 80

We Run Command for build image

CMD : docker build -t nginximage .

once Image Create then We run Container

CMD : docker run -d -p 8080:80 --name nginxcontainer nginximage

now check on browser

localhost:8080
