FROM alpine
RUN apk update && apk upgrade 
RUN apk add nginx
COPY ./index.nginx-debian.html /var/www/html/index.html
#COPY ./nginx.conf /etc/nginx/nginx.conf
COPY ./default /etc/nginx/http.d/default.conf
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
