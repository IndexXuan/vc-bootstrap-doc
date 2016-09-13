---
title: vc-animate
type: guide
order: 30
---

* [github](https://github.com/iwaimai-bi-fe/vc-animate)
* [npm](https://www.npmjs.com/package/vc-animate)
* [download](https://github.com/iwaimai-bi-fe/vc-animate/archive/master.zip)

## Install

```npm
npm install vc-animate --save
```

```html
//global varibale  vcanimate
<script src='../dist/vc-animate.js'></script>
```

## Usage

## props

### okText

custom the ok animate text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel animate text.

* default: `取消`
* type: `String`

### visiable

control the visiable of animate.

* default: `false`
* type: `Boolean` 

### onOk | optional

the callback for onOk.

* type: `Function`

### onCancel | optional

the callback of onCancel

* type: `Function`


## example

* js

```js
import Vue from 'vue'
import {
        vcanimate
    } from '../dist/vc-animate.js'

new Vue({
    el: '#app',
    data () {
        return {
            isShow: true,
            okText: 'ok',
            cancelText: 'cancel'
        }
    },
    components: {
        vcanimate
    },
    methods: {
        onOk () {

        },
        onCancel () {

        }
    },
    ready () {
    }
})
```

```vue
<vc-animate 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-animate>
```
