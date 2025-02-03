FROM node:17.9.0-slim
WORKDIR /app
RUN chown userui /app/home
RUN useradd userui
COPY . .
RUN npm install
USER userui
EXPOSE 3000
CMD [ "npm", "start" ]