FROM node:alpine

WORKDIR /app
COPY . /app

# RUN groupadd express && useradd -r -s /bin/false -G express express
# USER express

RUN npm install

ENV ATLAS_URI=mongodb://mongouser:mongopass@db
ENV PORT=5050

EXPOSE 5050

CMD ["npm", "start"]

