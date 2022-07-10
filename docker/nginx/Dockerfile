FROM nginx:1.21.6

LABEL linux=debian \
      server=nginx \
      app=web
COPY ./index.html /usr/share/nginx/html/
ADD ./nginx.conf /etc/nginx/nginx.conf

ENV  SERVICE_PORT=80
EXPOSE $SERVICE_PORT

ENTRYPOINT ["/usr/sbin/nginx"]
CMD ["-g", "daemon off;"]
