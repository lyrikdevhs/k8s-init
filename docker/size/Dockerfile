FROM nginx

COPY index.html /urs/share/nginx/html
ADD custom.conf /etc/nginx/conf.d/

EXPOSE 80

ENV FOO bar

CMD ["nginx", "-g", "daemon off;"]
