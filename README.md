# dockware/dev starting template

just a quick template to get started with dockware development

## Initial Setup
```bash
git clone git@github.com:emmathepossum/dockware.git
cd dockware
docker compose up -d
docker cp dockware:/var/www/html src
docker exec -it dockware composer install
git clone https://github.com/FriendsOfShopware/FroshDevelopmentHelper.git src/custom/plugins/FroshDevelopmentHelper
docker exec -it dockware bin/console plugin:install -ac FroshDevelopmentHelper
```


## Repeated Setup
```bash
docker compose up -d
```


## Connect to Container
```bash
docker exec -it dockware bash
```


see documentation:
- [dockware/dev](https://github.com/dockware/dockware/tree/master/.dist/versions/master/dev/latest)
- [Shopware Plugin Base Guide](https://developer.shopware.com/docs/guides/plugins/plugins/plugin-base-guide.html)
- [FroshDevelopmentHelper](https://github.com/FriendsOfShopware/FroshDevelopmentHelper)