FROM arm64v8/nginx
LABEL Project="Vprofile"
LABEL Author="Ferdie"

RUN rm -rf /etc/nginx/conf.d/default.conf
COPY nginxproapp.conf  /etc/nginx/conf.d/vprofile.conf
