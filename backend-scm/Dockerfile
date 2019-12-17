FROM node
WORKDIR /home/cfilth/lab-devops/backend-scm/
COPY package*.json ./
RUN npm install 
COPY . . 
EXPOSE 30030
CMD ["npm","start"]