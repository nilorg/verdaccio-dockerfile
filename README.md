# verdaccio-dockerfile
verdaccio npmjs proxy https://registry.npm.taobao.org

verdaccio部署简易私有化的npm包管理，已配置[npm-taobao](https://registry.npm.taobao.org)作为代理

sinopia已停止维护，改用[verdaccio](https://github.com/verdaccio/verdaccio)作为私有化的npm包管理

```bash
docker run --name verdaccio -e VERDACCIO_PORT=4873 -v /data/dockervolume/verdaccio/storage:/verdaccio/storage -p 4873:4873 -d nilorg/verdaccio

# debug
docker run -it --rm --name verdaccio -v ~/verdaccio/storage:/verdaccio/storage -p 4873:4873 nilorg/verdaccio
```
