## Vue-components
Component library for Vue 2.0+

### TanTan-slider
A Vue component that provides similar functionality to TanTan slider 

### Development
```
  # install dependencies
  npm install

  # run node server.js
  npm run server

  # build for production and view the bundle analyzer report
  npm run build --report
```
### Compatibility
- Vuejs(2.5.2)
- Modern browsers and IE10+

### Usage
```js
  //...
  <div class="stack-wrapper">
    <stack ref="stack" :pages="someList"/>
  </div>

  import stack from './components/stack'
```
props:

|Name| Default|Description|
|----|-----|-----|
| pages |[ ]| Binding of image src value |


```js
  pages: {
    type: Array,
    default: []
  }
```
template:

```html
    <li class="stack-item" v-for="(item, index) in pages"
      :style="[transformIndex(index),transform(index)]"
      @touchmove.stop.capture.prevent="touchmove"
      @touchstart.stop.capture.prevent="touchstart"
      @touchend.stop.capture.prevent="touchend"
      @touchcancel.stop.capture.prevent="touchend"
      @mousedown.stop.capture.prevent="touchstart"
      @mouseup.stop.capture.prevent="touchend"
      @mousemove.stop.capture.prevent="touchmove"
      @mouseout.stop.capture.prevent="touchend">
        <div v-html="item.html"></div>
    </li>
```


#### Introduction
[TanTan-slider](https://www.google.com.hk/search?newwindow=1&safe=strict&ei=5CohW7PdJ8ea0gSBupCIAg&q=markdown%E8%AF%AD%E6%B3%95+%E6%B0%B4%E6%99%B6&oq=markdown%E8%AF%AD%E6%B3%95+%E6%B0%B4%E6%99%B6&gs_l=psy-ab.3...2511.2511.0.3054.1.1.0.0.0.0.104.104.0j1.1.0....0...1c.1.64.psy-ab..0.0.0....0.9Z8MgrIed2I)

#### Demo

[preview](https://ws3.sinaimg.cn/large/006tNc79gy1fsah1hqys3g30sd0g4gtj.gif)