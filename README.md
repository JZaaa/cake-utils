CakeUtils
============
CakePHP3 助手

## Requires
- php: >=5.6
- cakephp/cakephp: ^3.7

## 安装

```
composer require jzaaa/cake-utils
```

## 开启CakePHP插件
```
bin/cake plugin load JZaaa/CakeUtils
```
或
```
// src/Application.php
public function bootstrap()
{
    parent::bootstrap();
    $this->addPlugin('JZaaa/CakeUtils');
}
```
## 助手内容

- [CakeBackup](./docs/CakeBackup.md) 简易数据库备份插件





