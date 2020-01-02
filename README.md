# Zenvia Package

This package was created in order to simplify the Zenvia API for those using it in several projects.

### Installation (with Composer)

```
composer require fabioaov/zenvia
```

### Setup

Add these variables to your *.env* file. Check out [PHP dotenv](https://github.com/vlucas/phpdotenv) if you don't have one.
```
ZENVIA_AUTH_TOKEN=
ZENVIA_SENDER_NAME=
```

### Usage

Just create a SMS instance:
```
use Fabioaov\Zenvia\SMS;

$zenvia = new SMS();
```
And call the method:
```
return $zenvia->sendSms($phoneNumber, $text);
```
