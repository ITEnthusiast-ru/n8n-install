FROM n8nio/n8n:latest

USER root
# установить ffmpeg и tzdata, настроить таймзону (пример Europe/Moscow)
RUN apk add --no-cache ffmpeg tzdata \
 && cp /usr/share/zoneinfo/Europe/Moscow /etc/localtime \
 && echo "Europe/Moscow" > /etc/timezone

ENV TZ=Europe/Moscow

USER node
