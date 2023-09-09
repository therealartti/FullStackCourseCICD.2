FROM node:16

WORKDIR /usr/src/todo-frontend

COPY . .

RUN npm ci

RUN CI=true npm test

RUN npm run build

RUN npm install -g serve
CMD ["serve", "build"]