FROM node:17.5-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npx prisma generate

EXPOSE 3000
CMD ["npm", "run", "dev"]