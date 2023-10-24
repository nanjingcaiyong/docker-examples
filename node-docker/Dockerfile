FROM node:16-alpine3.15

# 在镜像中创建一个文件夹存放应用程序代码，这将是你的应用程序工作目录
WORKDIR /Users/caiyong/Desktop/demos/docker-demo/work

# 此镜像中 Node.js 和 NPM 都已经安装，所以下一件事对于我们而言是使用 npm 安装你的应用程序的所有依赖。请注意，如果你的 npm 的版本是 4 或者更早的版本，package-lock.json 文件将不会自动生成。

COPY package.json ./
RUN npm install

# 

COPY . .

# 你的应用程序绑定的端口为 8080，所以你可以使用 EXPOSE 命令使它与 docker 的镜像做映射：
EXPOSE 8089

CMD [ "node", "server.js" ]