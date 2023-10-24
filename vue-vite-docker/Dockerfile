# 使用 Nginx 作为基础镜像
FROM nginx

# 删除默认的 Nginx 配置文件
RUN rm /etc/nginx/conf.d/default.conf

# 将本地的 Nginx 配置文件复制到容器中
COPY nginx.conf /etc/nginx/conf.d/

# 将静态文件复制到 Nginx 默认的静态文件目录
COPY dist /usr/share/nginx/html

# 暴露 Nginx 端口（默认为 80）
EXPOSE 80