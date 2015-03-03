# bullseye

> Attach elements onto their target

# Install

```shell
npm install bullseye --save
```

```shell
bower install bullseye --save
```

# `bullseye(el, target, options?)`

Position `el` according to the current position of `target`. If the `tracking` option isn't set to `false`, a listener for window resize events will make sure `el` stays well-position when the viewport size changes.

When you call `bullseye(el, target, options?)`, you'll get back a tiny API to interact with the instance.

### `.refresh()`

Refreshes position of `el` according to the current position of `target`.

### `.destroy()`

Removes the `resize` event listener. Note that further calls to `.refresh` will throw exceptions.

# License

MIT
