# proxy-server

axios, puppeteer 크롤링시 ip 우회를 위한 프록시 서버

<br/>

## Getting Started

```
docker build . --tag nginx-forward-proxy:0.0.1
docker run -d -p 3128:3128 --name proxy-server --restart=always nginx-forward-proxy:0.0.1
```

## Test

```
curl https://github.com/ -v -x 127.0.0.1:3128
```
