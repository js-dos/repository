# Repository of Dos.Zone

Ultimate collection of free js-dos bundles.

## How to build

1. yarn && cd sls && yarn && cd ..
2. yarn run build

## How to deploy

For aws:

```
yarn run build && cd _site && aws s3 sync --acl public-read . s3://dos.zone && cd ..
```

For yandex:

```
yarn run build && cd _site && aws s3 --endpoint-url=https://storage.yandexcloud.net sync --acl public-read . s3://dos.zone && cd ..
```

Optionally you can specify --delete in (3), if so you need to redeploy dos.zone.app.



