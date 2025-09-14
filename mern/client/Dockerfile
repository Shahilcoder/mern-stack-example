FROM node:alpine

WORKDIR /app
COPY . /app

# RUN groupadd react && useradd -r -s /bin/false -G react react
# USER react

RUN npm install
RUN npm install -g serve
RUN npm run build

EXPOSE 3000

CMD ["serve", "-s", "dist", "-l", "3117"]

