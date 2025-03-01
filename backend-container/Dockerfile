FROM node:20 
EXPOSE 8080
ENV DB_HOST=mysql
RUN useradd expense 
RUN mkdir /opt/app
RUN chown expense:expense -R /opt/app
WORKDIR /opt/app
COPY package.json .
COPY *.js .
RUN npm install 
CMD [ "node","index.js" ]