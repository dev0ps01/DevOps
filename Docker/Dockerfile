FROM  ubuntu
RUN   apt update
RUN   apt install nginx -y
CMD   ["nginx", "-g", "daemon off;"]
LABEL Name="vamsi"\
      Surname="Akkala"\
#EXPOSE  80
ENV    URL="google.com"
ENV    project="vamsi"
ADD    rm -rf  /var/www/html/*
ADD    index.html  /var/www/html
