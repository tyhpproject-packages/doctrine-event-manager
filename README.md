<!-- tyhp-readme:start -->
# tyhpdef/doctrine-event-manager

Tyhp type definitions for `doctrine/event-manager` `2.1.1`.

```bash
composer require --dev tyhpdef/doctrine-event-manager:2.1.1
```

This is a metapackage. Composer also installs `tyhpdef/doctrine-event-manager-impl` (type files).
Require **this** name, not `tyhpdef/doctrine-event-manager-impl`.

See https://tyhplang.com.

## Maintain `doctrine/event-manager`? Ship the types yourself

If you are a Packagist maintainer of `doctrine/event-manager`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/doctrine-event-manager-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `doctrine/event-manager` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/doctrine-event-manager": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `doctrine/event-manager` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `doctrine/event-manager` with a real constraint,
   `"replace": { "tyhpdef/doctrine-event-manager": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `doctrine/event-manager` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/doctrine-event-manager` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
