---
title: vc-radio
type: guide
order: 7
---

* [github](https://github.com/iwaimai-bi-fe/vc-radio)
* [npm](https://www.npmjs.com/package/vc-radio)
* [download](https://github.com/iwaimai-bi-fe/vc-radio/archive/master.zip)

## Install

```npm
npm install vc-radio --save
```

```html
//global varibale  vcradio
<script src='../dist/vc-radio.js'></script>
```

## Usage

## props

### okText

custom the ok radio text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel radio text.

* default: `取消`
* type: `String`

### visiable

control the visiable of radio.

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
        vcradio
    } from '../dist/vc-radio.js'

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
        vcradio
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
<vc-radio 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-radio>
```
