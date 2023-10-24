## 打包

### 构建

```sh
npm run build
```

### 部署

```sh
docker build -t vue-nginx .
docker run -d -p 8081:80 vue-nginx 
```