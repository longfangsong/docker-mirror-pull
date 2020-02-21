# docker-mirror-pull
docker pull from mirror site [azk8s.cn](azk8s.cn)
## install
```shell
curl https://raw.githubusercontent.com/longfangsong/docker-mirror-pull/master/docker-mirror-pull > ./docker-mirror-pull
chmod +x ./docker-mirror-pull
# AND maybe you want to export it into PATH
sudo mv ./docker-mirror-pull /usr/local/bin/
```

## upgrade

```shell
curl https://raw.githubusercontent.com/longfangsong/docker-mirror-pull/master/docker-mirror-pull > ./docker-mirror-pull
chmod +x ./docker-mirror-pull
# AND maybe you want to upgrade it in $PATH
sudo mv ./docker-mirror-pull /usr/local/bin/
```

## use
Just replace all `docker pull` with `docker-mirror-pull`, eg.
```shell
docker-mirror-pull alpine
```
This will pull `dockerhub.azk8s.cn/library/alpine` image, retag the image as `alpine`, and then remove  `dockerhub.azk8s.cn/library/alpine`.

Currently this script supports images from `dockerhub`, `quay.io` and `gcr.io`.
