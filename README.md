
### Installation by composer
###
```
{
    "require": {
      "apolon13/yii2-sftp-phpseclib": "dev-master"
   }
}
```
 ### or
 ###

>$ composer require apolon13/yii2-sftp-phpseclib

### USAGE
###
```
'components' => [
      ...
      'sftp' => [
          "class" => 'Apolon\sftp\SFtpManager',
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

### documentation
http://phpseclib.sourceforge.net/index.html




License
----

MIT
