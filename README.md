Laravel IDE support

> I don't want to install `barryvdh/laravel-ide-helper` in every Laravel project, even as a dev dependency. Therefore, I create this repository to provide a simple solution to generate meta files for IntelliJ IDEA which I'm using. In another word, this solution still depends on `barryvdh/laravel-ide-helper`, but is kept independently of my source code.

## Usage

1. Go to a Laravel project that already has vendor directory (after running composer install)
```bash
cd /path/to/laravel
``` 

2. Clone this repository into `vendor/_ide_support` directory.

```bash
git clone https://github.com/seriquynh/laravel-ide-support.git vendor/_ide_support
```

3. Install dependencies inside `vendor/_ide_support` directory, not the project base directory.

```bash
composer install -d ./vendor/_ide_support
```

4. Execute the composer `support` script in `vendor/_ide_support` directory.

```bash
composer run support -d ./vendor/_ide_support
```
