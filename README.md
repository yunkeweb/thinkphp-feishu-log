<h1 align="center"> thinkphp-feishu-log </h1>

<p align="center"> 基于thinkphp的飞书日志扩展.</p>


## Installing

```shell
$ composer require yunkeweb/thinkphp-feishu-log -vvv
```

## Usage

安装之后，在 `config/log.php` 文件中的`channels`数组中新增以下配置:
```php
'fei_shu' => [
    'type' => \Yunkeweb\ThinkphpFeiShuLog\FeiShu::class,
    'title' => '项目报警日志',
    'webhook' => '', // 飞书机器人 webhook 地址
    'secret_key' => '', // 安全设置签名校验 密钥
]
```

## Contributing

You can contribute in one of three ways:

1. File bug reports using the [issue tracker](https://github.com/yunkeweb/thinkphp-feishu-log/issues).
2. Answer questions or fix bugs on the [issue tracker](https://github.com/yunkeweb/thinkphp-feishu-log/issues).
3. Contribute new features or update the wiki.

_The code contribution process is not very formal. You just need to make sure that you follow the PSR-0, PSR-1, and PSR-2 coding guidelines. Any new code contributions must be accompanied by unit tests where applicable._

## License

MIT