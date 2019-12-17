FROM node
WORKDIR /home/cfilth/lab-devops/backend-user/
COPY package*.json ./
RUN npm install 
COPY . . 
EXPOSE 3020
CMD ["npm","start"]