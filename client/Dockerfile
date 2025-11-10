FROM node:20-alpine

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .
ENV VITE_API_URL=http://localhost:5000/api
RUN npm run build

EXPOSE 5173

CMD ["npm", "run", "preview"]

