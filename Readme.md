*This repository is a mirror of the [component](http://component.io) module [segmentio/chrome-events](http://github.com/segmentio/chrome-events). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/segmentio-chrome-events`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# chrome-events

  tiny wrapper for chrome events, inspired by component/events

## Installation

  Install with [component(1)](http://component.io):

    $ component install segmentio/chrome-events

## Example

```js

var events = require('chrome-events');

function App(){
  this.events = events(chrome.runtime, this);
  this.events.bind('installed');
  this.events.bind('startup');
  this.events.bind('suspend');
  this.events.bind('message');
}

App.prototype.oninstalled = function(){};
App.prototype.onstartup = function(){};
App.prototype.onsuspend = function(){};
App.prototype.onmessage = function(){};

```

## License

  MIT
