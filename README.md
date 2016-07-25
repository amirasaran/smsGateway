# smsGateway

Turn your Android phone into a SMS Gateway
----------

Send and receive messages programmatically through your phone using API service

   - first register for free  [login/signup](https://smsgateway.me/admin/users/login)
   - read [documentation](https://smsgateway.me/admin/users/login)
   - [smsgateway.me](https://smsgateway.me/)

How to install 
--------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require amirasaran/smsGateway:dev-master
```

or add

```
"amirasaran/smsGateway": "dev-master"
```


How to Use
----------

```sh
....
$login = [
    'username' => 'Your-Email@Exmaple.com',
    'password' => 'YourPassword'
];
$smsGateway = new amirasaran\smsgateway\SmsGateway($login);
$devices = $smsGateway->getDevices();

var_dump($devices);

...
```