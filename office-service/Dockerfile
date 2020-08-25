FROM node:lts-alpine3.10

RUN apk add docker make bash git  

WORKDIR /project-assessment-site 
COPY package.json /project-assessment-site
RUN npm install 
COPY . /project-assessment-site

ENTRYPOINT ["node"]

CMD ["index.js"]

EXPOSE 80
