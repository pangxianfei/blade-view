# think-view

ThinkPHP8.0 Think-Template模板引擎驱动


## 安装

~~~php
composer require tmaic/blade-view
~~~

## 用法示例

本扩展不能单独使用，依赖ThinkPHP8.0+

首先配置config目录下的view.php配置文件，然后可以按照下面的用法使用。

~~~php
<?php
[
    // 模板引擎类型
    'type'         => 'blade',
    // 默认模板渲染规则 1 解析为小写+下划线 2 全部转换小写 3 保持操作方法
    'auto_rule'    => 1,
    // 模板目录名
    'view_dir_name'=> 'view',
    // 模板后缀
    'view_suffix'  => 'blade.php',
    // 模板文件名分隔符
    'view_depr'    => DIRECTORY_SEPARATOR,
    // 编译缓存
    'tpl_cache'     => true,
];

~~~

具体的如何使用参考laravel blade模板引擎