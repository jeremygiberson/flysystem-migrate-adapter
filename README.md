# Flysystem Adapter for Migration.

## Installation

```bash
composer require jeremygiberson/flysystem-migrate-adapter
```

## Usage

```php
$source = new League\Flysystem\Adapter\AwsS3(...);
$replica = new League\Flysystem\Adapter\Local(...);
$adapter = new JeremyGiberson\Flysystem\Migrate\MigrateAdapter($source, $replica);
```