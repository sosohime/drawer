# rc-drawer
---

[![NPM version][npm-image]][npm-url]
[![build status][travis-image]][travis-url]
[![codecov](https://codecov.io/gh/react-component/drawer/branch/master/graph/badge.svg)](https://codecov.io/gh/react-component/drawer)
[![node version][node-image]][node-url]
[![npm download][download-image]][download-url]

[npm-image]: http://img.shields.io/npm/v/rc-drawer.svg?style=flat-square
[npm-url]: http://npmjs.org/package/rc-drawer
[travis-image]: https://img.shields.io/travis/react-component/drawer.svg?style=flat-square
[travis-url]: https://travis-ci.org/react-component/drawer
[node-image]: https://img.shields.io/badge/node.js-%3E=_0.10-green.svg?style=flat-square
[node-url]: http://nodejs.org/download/
[download-image]: https://img.shields.io/npm/dm/rc-drawer.svg?style=flat-square
[download-url]: https://npmjs.org/package/rc-drawer

## Example

http://react-component.github.io/drawer/examples/

## Usage

```js
import Drawer from 'rc-drawer';
import React from 'react';
import ReactDom from 'react-dom';

ReactDom.render(
  <Drawer>
    {menu children}
  </Drawer>
, mountNode);
```

## Install

[![rc-drawer](https://nodei.co/npm/rc-drawer.png)](https://npmjs.org/package/rc-drawer)

## Browser Support

|![IE](https://github.com/alrra/browser-logos/blob/master/src/edge/edge_48x48.png?raw=true) | ![Chrome](https://github.com/alrra/browser-logos/blob/master/src/chrome/chrome_48x48.png?raw=true) | ![Firefox](https://github.com/alrra/browser-logos/blob/master/src/firefox/firefox_48x48.png?raw=true) | ![Opera](https://github.com/alrra/browser-logos/blob/master/src/opera/opera_48x48.png?raw=true) | ![Safari](https://github.com/alrra/browser-logos/blob/master/src/safari/safari_48x48.png?raw=true)|
| --- | --- | --- | --- | --- |
| IE 10+ ✔ | Chrome 31.0+ ✔ | Firefox 31.0+ ✔ | Opera 30.0+ ✔ | Safari 7.0+ ✔ |

## API

| props      | type           | default | description    |
|------------|----------------|---------|----------------|
| className       | string | null | - |
| prefixCls     |  string  | 'drawer' | prefix class |
| wrapperClassName | string | null | wrapper class name |
| open        | boolean  | false |  open or close menu  |
| defaultOpen | boolean  | false | default open menu |
| handler   | boolean \| ReactElement | true | true or false or ReactElement, default:  `<divclassName="drawer-handle"><i className="drawer-handle-icon" /></div>`;  |
| placement  | string   |  `left` | `left` `top` `right` `bottom` |
| level     | string \| array | `all` | With the drawer level element. `all`/ null / className / id / tagName / array |
| levelMove | number \| array \| func | null |level move value. default is drawer width |
| duration | string | `.3s` | level animation duration |
| ease | string | `cubic-bezier(0.78, 0.14, 0.15, 0.86)` | level animation timing function |
| getContainer    | string \| func \| HTMLElement | `body` | Return the mount node for Drawer. if is `null` use React.creactElement  |
| showMask    |  boolean  | true | mask is show |
| maskStyle | object | null | mask style |
| onChange  | func | null | change callback(open) |
| onMaskClick | func | null | mask close click function |
| onHandleClick | func | nul  | handle icon click function |

> 1.5 Rename `handleChild` -> `handler`, remove `handleStyle`, remove `levelTransition` -> `duration` `ease`, add `levelMove`.
## Development

```
npm install
npm start
```
