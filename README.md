# videojs-basic

Videojs Basic Plugin empty by generator-videojs-plugin

## Installation

```sh
npm install --save videojs-basic
```

## Usage

To include videojs-basic on your website or web application, use any of the following methods.

### `<script>` Tag

This is the simplest case. Get the script in whatever way you prefer and include the plugin _after_ you include [video.js][videojs], so that the `videojs` global is available.

```html
<script src="//path/to/video.min.js"></script>
<script src="//path/to/videojs-basic.min.js"></script>
<script>
  var player = videojs('my-video');

  player.basic();
</script>
```

### Browserify/CommonJS

When using with Browserify, install videojs-basic via npm and `require` the plugin as you would any other module.

```js
var videojs = require('video.js');

// The actual plugin function is exported by this module, but it is also
// attached to the `Player.prototype`; so, there is no need to assign it
// to a variable.
require('videojs-basic');

var player = videojs('my-video');

player.basic();
```

### RequireJS/AMD

When using with RequireJS (or another AMD library), get the script in whatever way you prefer and `require` the plugin as you normally would:

```js
require(['video.js', 'videojs-basic'], function(videojs) {
  var player = videojs('my-video');

  player.basic();
});
```

## License

MIT. Copyright (c) Tank.vn


[videojs]: http://videojs.com/
