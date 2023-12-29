FROM node:slim

ADD ./app/ /app/
ADD ./docker-entrypoint-wrapper.sh /script/

WORKDIR /app

RUN npm install

EXPOSE 80

#CMD [ "/script/docker-entrypoint-wrapper.sh" ]
ENTRYPOINT ["bash","-c","/script/docker-entrypoint-wrapper.sh"]