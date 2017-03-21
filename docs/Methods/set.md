# Set

## keystone.set(key:String, value:Mixed)

`keystone.set` provides an option to keystone for use during keystone setup. Assigns the value provided to the key in keystone's options object. `keystone.set` returns the value object.

You should not set keystone options after keystone has been started.

The initialization options can be found in the [configuration](/configuration) documentation.

For information on setting up keystone, see the [installation guide](/guides/setting-up/installation)

Example:

```javascript
keystone.set('port', 5050)
```

There are middleware that can be added with `set` which will be automatically run for particular actions. For information on these see the [middleware](/methods/middleware) documentation.

`keystone.set(key:string)` - .set can also be called with a string and no value passed in. If there is only one argument, `keystone.set` will instead retrieve the value of the selected key from keystone. This is aliased as [keystone.get()](/methods/get),