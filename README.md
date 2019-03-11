# laravel-running-time

![Image](https://github.com/y-ui/y-ui.github.io/blob/master/table.png)

## Installation

    composer require y-ui/laravel-running-time 0.1
    
## Configuration

1. Open your `app/Console/Kernel.php` and add the following to the `$commands` array:

    ```php
    \RunningTime\Command\RunningTimeCommand::class,
    ```
    
2. Open your `app/Http/Kernel.php` and add the following to `$middleware` array:

    ```php
    \RunningTime\Middleware\RunningTimeMiddleware::class,
    ```

## Usage
### Simple usage
```shell
php artisan running-time
```

This will count the last 7 days of data

### Options

    --line  Maximum number of displayed lines
    --start Statistical start time
    --end   Statistical end time
    
    
## TODO LIST
 
- Delayed batch write
- More statistical tools
- Web page
- Config support
