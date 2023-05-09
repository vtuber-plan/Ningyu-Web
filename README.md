## Ningyu Web

本 Fork 适配 FastChat 接口

1. 安装
```
git clone https://github.com/vtuber-plan/Ningyu-Web
sudo docker build -t ningyu_web:latest .
```

2. 启动
```shell
sudo docker run -d -p 3000:3000 \  
      -e OPENAI_API_KEY="sk-xxxx" \
      -e CODE="test" \
      -e BASE_URL="127.0.0.1:8000"\
      -e PROTOCOL="http"\
      --net=host\
   docker.io/library/ningyu_web:latest
```