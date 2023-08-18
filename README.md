# WordPress Utils

A simple utils plugin that lets you register the same handler to multiple filters without much effort.

## Installation

### If you use a Roots Bedrock or a composer-based WordPress installation

```bash
composer require dartmoon/wordpress-utils
```

## If you use a normal WordPress installation

1. Download and install a MU plugin loader that lets you use MU plugins that resides inside folders. For example you could use [Bedrock Autoloader](https://github.com/roots/bedrock-autoloader).

2. [Download the latest release](https://github.com/dartmoon-io/wordpress-utils/releases) of this plugin and extract it inside the mu-plugins folder of your WordPress installation.

## Usage
It behave exactly as `add_filter` with the only exception that the first argument (the filter name) accepts an array instead of a string.

```php
add_filters(['filter1', 'filter2'], function () {
    // ...
});
```

## License

This project is licensed under the MIT License - see the LICENSE.md file for details