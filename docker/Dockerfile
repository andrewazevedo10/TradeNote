FROM node:18-alpine3.17
RUN apk add --no-cache bash
WORKDIR /app
COPY package.json package-lock.json .
ADD ./ .
RUN npm install
RUN npm run build
CMD ["npm", "start"]
