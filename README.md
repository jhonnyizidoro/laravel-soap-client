# How to use?

```php
use App\Helpers\SoapClient;

$response = SoapClient::wsdl('https://github.com/service?wsdl')
->parameters([
  'LOGIN' => [
    'USER' => 'jhonnyizidoro',
    'PASSWORD' => 'secret'
  ]
])
->call('USER_LOGIN');
```

## Available options
```php
SoapClient::wsdl('wsdl url')
->parameters(['array of data'])
->call('function to call');
->location('location url')
->trace('boolean')
->exception('boolean')
->timeout('time in sec');
```
