FROM node as builder
ARG NPM_ENV=development
WORKDIR /home/cfilth/lab-devops/frontend/
COPY package*.json ./
RUN npm install 
COPY src/ ./src/
COPY public/ ./public/
RUN npm run build:${NPM_ENV}
FROM nginx 
COPY --from=builder /home/cfilth/lab-devops/frontend/build/ /usr/share/nginx/html
EXPOSE 80 