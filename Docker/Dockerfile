FROM  ubuntu
RUN   apt update
RUN   apt install nginx -y
CMD   ["nginx", "-g", "daemon off;"]
LABEL Name="vamsi"\
      Surname="Akkala"\
#EXPOSE  80
ENV    URL="google.com"
ENV    project="vamsi"
RUN    rm -rf  /var/www/html/*
#ADD    index.html  /var/www/html/index.html
#you can change ownership of the file using --chown=user
ADD    html  /var/www/html
# if you mention directory it will copy the files inside that directory to the declared path
#  inside that if you have other directory it will copy that one also

