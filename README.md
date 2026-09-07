# CMS Canonical for Magento 2 (SISL fork)

Adds a `<link rel="canonical">` tag to Magento 2 CMS pages — closing a common on-page SEO gap,
since Magento does not add canonicals to CMS pages out of the box.

Maintained fork of `hhennes/module-cms`, verified on **Magento 2.4.9 / PHP 8.4**.

## What changed vs upstream

- Added `require` to composer.json (`php` 8.1–8.5, `magento/framework >=103.0.4 <104`).
  The original declared no requirements, so Composer would install it on any incompatible
  version silently.

## Install

```bash
composer config repositories.cmscanon vcs https://github.com/SISL-source/magento2-cms-canonical
composer require hhennes/module-cms:dev-main
bin/magento setup:upgrade
```

## License

AFL-3.0 (upstream). Maintained by [SISL](https://sisl.pl).
