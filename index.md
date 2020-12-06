# index

## VScodeでxdebugを使う方法を検証
vs codeでXdebugを使う方法を検証してみた。
結論から言うと、以下のようにphp.iniを変更する感じ。

```php.ini
[XDebug]
zend_extension = C:\xampp\php\ext\php_xdebug-3.0.1-7.4-vc15-x86_64.dll
xdebug.mode = develop,debug
xdebug.start_with_request = yes
xdebug.remote_enable = 1
xdebug.remote_autostart = 1
xdebug.remote_connect_back = 1
xdebug.remote_port = 9000
xdebug.client_port = 9000
```
