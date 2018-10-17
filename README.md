GSAP React Native Plugin
=================

A [GSAP] plugin for tweening [ReactNative] component state.

Usage
-----

```javascript
require('gsap');
require('gsap-react-native');

React.createClass({
    getInitialState: function() {
        return {width: 0};
    },
    componentDidMount: function() {
        TweenLite.to(this, 1, {state: {width: 100}});
    },
    render: function() {
        return <div style={{width: this.state.width}}>Hello World!</div>
    }
});
```


Installation
------------
- Via [npm]: `npm install gsap && npm install gsap-react-native`
- Via file > save as: [gsap-react-native.js]

[GSAP]: http://www.greensock.com/gsap-js/
[React.js]: http://facebook.github.io/react/
[npm]: http://npmjs.org
[bower]: http://bower.io
[gsap-react-plugin.js]: https://raw.githubusercontent.com/hzdg/gsap-react-plugin/master/gsap-react-plugin.js
