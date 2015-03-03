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

In order to play well with friends, bullseye won't change the `position` CSS property, but instead leaves it up to you to set the appropriate `position` value on `el`. This way, we don't make it hard for you to set a different `position` value when you need to.

### `.refresh()`

Refreshes position of `el` according to the current position of `target`.

### `.destroy()`

Removes the `resize` event listener. Note that further calls to `.refresh` will throw exceptions.

# License

MIT
