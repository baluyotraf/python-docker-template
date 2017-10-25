FROM library/nginx:1.13.5

COPY web/ /opt/web/
COPY nginx/nginx.conf /etc/nginx/nginx.conf

CMD ["nginx", "-g", "daemon off;"]