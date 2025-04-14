FROM node:20-alpine

WORKDIR /app

COPY package*.json ./
COPY yarn*.lock ./

RUN yarn install --frozen-lockfile

COPY . .

ENV NODE_ENV=production
ENV PORT=8080

EXPOSE 8080

CMD ["yarn", "start"]