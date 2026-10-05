<!-- tyhp-readme:start -->
# tyhpdef/livewire-livewire

Tyhp type definitions for `livewire/livewire` `4.4.5`.

```bash
composer require --dev tyhpdef/livewire-livewire:4.4.5
```

This is a metapackage. Composer also installs `tyhpdef/livewire-livewire-impl` (type files).
Require **this** name, not `tyhpdef/livewire-livewire-impl`.

See https://tyhplang.com.

## Maintain `livewire/livewire`? Ship the types yourself

If you are a Packagist maintainer of `livewire/livewire`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/livewire-livewire-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `livewire/livewire` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/livewire-livewire": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `livewire/livewire` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `livewire/livewire` with a real constraint,
   `"replace": { "tyhpdef/livewire-livewire": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `livewire/livewire` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/livewire-livewire` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
