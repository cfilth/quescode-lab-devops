FROM node
WORKDIR /home/cfilth/lab-devops/backend-scm/
COPY package*.json ./
RUN npm install 
COPY . . 
EXPOSE 3030
CMD ["npm","start"]