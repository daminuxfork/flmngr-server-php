# Flmngr - file manager

> Module for PHP for server-side file management

Use Flmngr file manager to upload and manage files and images on your website. Works great together with [ImgPen](https://imgpen.com) which adds feature to edit images right from file manager.


## Install

With [Composer](https://getcomposer.org/) installed, run

```
$ composer require edsdk/flmngr-server-php
```


## Usage

To handle some URL you want in your web application, create a file which will be entry point for all requests, e. g. `file-manager.php`: 

```php
<?php

    require __DIR__ . '/../vendor/autoload.php';
    
    use EdSDK\FlmngrServer\Flmngr;
    
    Flmngr::flmngrRequest(
        array(
            'dirFiles' => 'path-to/files',
            'dirTmp'   => 'path-to/tmp',
            'dirCache'   => 'path-to/cache'
        )
    );
```

If you want to allow access to uploaded files (usually you do) please do not forget to open access to files directory.

Please also see [example of usage](https://packagist.org/packages/edsdk/flmngr-example-php) Flmngr with ImgPen for editing and uploading images.


## Server languages support

Current package is targeted to serve uploads inside PHP environment.

Another backends are also available:

- Node (TypeScript/JavaScript)
- PHP
- Java


## See Also

- [N1ED](https://n1ed.com) - you can integrate Flmngr with N1ED HTML editor
- [ImgPen website](https://n1ed.com/docs/addons/image-editor) - image editor for Flmngr


## License

Commercial EdSDK license. Purchase the product in order to use it.