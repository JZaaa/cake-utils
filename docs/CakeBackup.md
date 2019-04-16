CakeBackup
==========
简易数据库备份插件，当前仅支持`Mysql`

## 使用

### 示例

```
use JZaaa\CakeUtils\Lib\CakeBackup;

// 实例化
$driver = CakeBackup::getInstance();

// 备份数据库
$driver->backupDB();

```

### 配置

数据库默认保存路径为`/config/backupsql`,获取`mysql`连接为CakePHP`default`。
```
// 自定义
CakeBackup::getInstance($path, $datasources);
```

### 方法

| 方法       |   参数   | 注释 |
| :--:       |  :--:    | :--: |
| getDriver  | --       |  获取数据库类型   |
| getTableStatus  | --       |  获取所有表状态   |
| getTableList  | --       |  获取所有表名   |
| getTableInfo  |  {string} 表名       |   获取表信息  |
| optimize  |  {string\|array} 表名,例：table1,table2 或 \[table1,table2]     |   优化表  |
| repair  |  {string\|array} 表名,例：table1,table2 或 \[table1,table2]     |   修复表,注意仅MyISAM表可用  |
| backupTables  |  {array} 表名,例：\[table1,table2]     |   数据表备份  |
| backupDB  |  --     |   数据库备份  |

## 其他
该类仅建议在数据库较小时使用。


