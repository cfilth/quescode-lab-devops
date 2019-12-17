FROM node as builder
WORKDIR /home/cfilth/lab-devops/frontend/
COPY package*.json ./
RUN npm install 
COPY src/ ./src/
COPY public/ ./public/
RUN npm run build
FROM nginx 
COPY --from=builder /home/cfilth/lab-devops/frontend/build/ /usr/share/nginx/html
EXPOSE 80 
