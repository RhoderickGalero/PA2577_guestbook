# pull official base image
FROM node:16-alpine

# copy files/directories
ADD . /frontend

# set work directory
WORKDIR /frontend

# install dependencies
RUN npm install --silent

# launch the app 
CMD ["npm", "start"]