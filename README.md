# [PHP-CS-Fixer](https://github.com/PHP-CS-Fixer/PHP-CS-Fixer) config for [REDAXO](https://github.com/redaxo/redaxo)

### Installation

```
composer require --dev redaxo/php-cs-fixer-config
```

Example `.php-cs-fixer.dist.php`:

```php
<?php

use PhpCsFixer\Finder;
use Redaxo\PhpCsFixerConfig\Config;


$finder = (new Finder())
    ->in(__DIR__)
;

return Config::redaxo5() // or `::redaxo6()`
    ->setFinder($finder)
;

```
