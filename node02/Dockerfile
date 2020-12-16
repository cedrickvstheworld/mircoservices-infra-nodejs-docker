FROM node:10-slim
WORKDIR /usr/src/app
COPY package.json .
RUN npm install
COPY . .
RUN npm install -g typescript
RUN tsc
RUN rm -R src/
CMD ["npm", "run", "start"]
