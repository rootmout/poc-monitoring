FROM nginx:1.17
COPY nginx.conf /etc/nginx/nginx.conf
WORKDIR /nginx
COPY metrics .
EXPOSE 8080/tcp
RUN apt-get update
RUN apt-get install -y vim
CMD ["nginx", "-g", "daemon off;"]
