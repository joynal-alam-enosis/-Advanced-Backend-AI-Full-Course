FROM node 

#each line called layer
#docker chace all layers
#if one layer changes all layers after this will update including this

#create working direactory
WORKDIR /app

#copy
# COPY package*.json package.json
# COPY package-lock.json package-lock.json
COPY package*.json .

#run cmd  -> for Optimization
RUN npm install


#COPY index.js index.js

#files add in .dockerignore will not be copied

# copy all file
COPY . .

#to run
CMD [ "node", "index.js" ]
 