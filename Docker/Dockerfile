FROM  ubuntu
RUN   apt update
RUN   apt install nginx -y
# override the default command
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
ENTRYPOINT  ["ping", " -c", "2"]
VOLUME      /myvol
RUN      mkdir vamsi
RUN      useradd sample
USER     sample
ARG      URL
ENV      URL=${URL}
#  we can pass valuse through command using --build-arg URL=google.com
#  we can use it as variable
ONBUILD  ENV  URL=example.com
# if someone is trying to build on my image it will trigger an intruction
#kill -l gives all the signals in os
# we can use dockerfile name as different but when you are using in clu mention it with -f
# through cli we can override the entrypoint by using --entrypoint


