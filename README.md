# CI4 App Starter
```
composer create-project codeigniter4/appstarter <nome> --no-dev
```
```
composer config minimum-stability dev
```
```
composer require --no-update codeigniter4/shield
```
```
composer require --no-update rahpt/ci4-commands
```
```
composer require --no-update tatter/visits
```
```
composer update --no-dev
```

Após instalar, corra o migration para criar as tabelas
```
spark migrate --all
```
```
spark shield:setup
```
crie o utilizador ADMIN
```
spark shield:user create -n Admin -e admin@admin.com
```

adicione em um grupo admin
```
spark shield:user addgroup -n Admin -g admin
```

ativa o usuario
```
spark shield:user activate -n Admin
```
