FROM node:0.10
# Create app directory
WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install -d

COPY . .

RUN npm run build
#RUN cd nxAdmin  && npm install  --registry=http://registry.npm.taobao.org  && npm run build:prod

EXPOSE 7111

# RUN echo "Asia/Shanghai" > /etc/timezone
# RUN dpkg-reconfigure -f noninteractive tzdata

# RUN mkdir -p ./public/apidoc
# RUN apidoc -i ./router/v1 -o ./public/apidoc/

CMD [ "npm","run", "app" ]