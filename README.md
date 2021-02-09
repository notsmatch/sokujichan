# sokujichan

[WIP] No releases there.

8dx 6v6 score calculation discord bot with docker.

![](https://i.gyazo.com/93b7c2095bee49f17134e9018a11463e.jpg)

`docker-compose.yml`
```yml
version: '3.8'

services:
  sokujichan:
    container_name: sokujichan
    image: iamtakagi/sokujichan:latest
    restart: always
    ports:
      - 8080:8080
    environment:
      # Bot Token (Required)
      BOT_TOKEN: XXX
      # Base Uri
      BASE_URI: /
      # Server Host
      HOST: 0.0.0.0
      # Server Port
      PORT: 8080
      # Logger
      LOG: INFO
      # Embed color
      EMBED_COLOR: 83,221,172
```

```
# イメージ更新 / Update
docker pull iamtakagi/sokujichan:latest

# 起動 / Start
docker-compose up -d
```
