PDOSessionBundle
================

PDO Session Bundle adds PDO Session to your symfony project easy and fast.

Instal the bundle with composer

```json
...
"require": {
    ...
    "ferrandini/pdo-session-bundle": "1.*"
}
...
```

Enable the bundle in your `app/AppKernel.php`

```php
// app/AppKernel.php

...
    $bundles = array(
        ...
        new Ferrandini\Bundle\PDOSessionBundle\FerrandiniPDOSessionBundle(),
    );
...
```

Configure your session hanlder in `config.yml`

```yml
...
framework:
    ...
    session:
        handler_id: ferrandini.pdo.session.handler
...
```