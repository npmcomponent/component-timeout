*This repository is a mirror of the [component](http://component.io) module [component/timeout](http://github.com/component/timeout). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/component-timeout`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# timeout

  Timeout function decorator

## Installation

    $ component install component/timeout

## Example

```js
var timeout = require('timeout');

function something(fn) {
  setTimeout(function(){
    fn(null, 'results');
  }, 1000);
}


something = timeout(something, 500);
```

## API

### timeout(callback, ms)

  Apply timeout of `ms` to `callback` and return the new function.

## License

  MIT
