<!-- tyhp-readme:start -->
# tyhpdef/stripe-stripe-php

Tyhp type definitions for `stripe/stripe-php` `21.3.2`.

```bash
composer require --dev tyhpdef/stripe-stripe-php:21.3.2
```

This is a metapackage. Composer also installs `tyhpdef/stripe-stripe-php-impl` (type files).
Require **this** name, not `tyhpdef/stripe-stripe-php-impl`.

See https://tyhplang.com.

## Maintain `stripe/stripe-php`? Ship the types yourself

If you are a Packagist maintainer of `stripe/stripe-php`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/stripe-stripe-php-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `stripe/stripe-php` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/stripe-stripe-php": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `stripe/stripe-php` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `stripe/stripe-php` with a real constraint,
   `"replace": { "tyhpdef/stripe-stripe-php": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `stripe/stripe-php` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/stripe-stripe-php` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
