# * signifies all the files having package~~~~.json, here the left dot signifies the host 
# machine and right dot is container. we are copying all the package~~.json files from host to container.
# Run npm install, installs all dependencies in package.json
# then we copy all the source code from host to container

FROM node:16
WORKDIR /app
COPY ./package*.json ./      
RUN npm install             
COPY . .

CMD ["npm", "run", "dev"]