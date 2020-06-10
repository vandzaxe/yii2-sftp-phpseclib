
### Installation by composer
###
```
{
    "require": {
      "vandzaxe/yii2-sftp-phpseclib": "dev-master"
   }
}
```
 ### or
 ###

>$ composer require vandzaxe/yii2-sftp-phpseclib

### USAGE
###
```
'components' => [
      ...
      'sftp' => [
          "class" => 'Vandzaxe\sftp\SFtpManager',
          "settings"=>[
              'port'=>22,
              'timeout'=>10
            ]
       ],
 ],
 
$sftp = Yii::$app->sftp
$sftp->connect("host","user","pass");
echo $sftp->isConnected();
```

## Documentation

* [Documentation / Manual](http://phpseclib.sourceforge.net/)
* [API Documentation](https://api.phpseclib.org/master/) (generated by Sami)




License
----

MIT
