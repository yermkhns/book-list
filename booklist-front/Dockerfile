FROM node:18-slim

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

EXPOSE 5173

ENV VITE_HOST=0.0.0.0
ENV VITE_PORT=5173

CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"] 