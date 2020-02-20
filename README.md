# docker-mirror-pull
docker pull from mirror site [azk8s.cn](azk8s.cn)
## install
```shell
curl https://raw.githubusercontent.com/longfangsong/docker-mirror-pull/master/docker-mirror-pull > $SOMEWHERE_IN_YOUR_PATH
chmod +x $SOMEWHERE_IN_YOUR_PATH/docker-mirror-pull
```

## upgrade

curl https://raw.githubusercontent.com/longfangsong/docker-mirror-pull/master/docker-mirror-pull > $(which docker-mirror-pull)

## use
Just replace all `docker pull` with `docker-mirror-pull`, eg.
```shell
docker-mirror-pull alpine
```
This will pull `dockerhub.azk8s.cn/library/alpine` image, retag the image as `alpine`, and then remove  `dockerhub.azk8s.cn/library/alpine`.

Currently this script supports images from `dockerhub`, `quay.io` and `gcr.io`.
