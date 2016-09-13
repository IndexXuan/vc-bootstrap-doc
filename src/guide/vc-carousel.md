---
title: vc-carousel
type: guide
order: 15
---

* [github](https://github.com/iwaimai-bi-fe/vc-carousel)
* [npm](https://www.npmjs.com/package/vc-carousel)
* [download](https://github.com/iwaimai-bi-fe/vc-carousel/archive/master.zip)

## Install

```npm
npm install vc-carousel --save
```

```html
//global varibale  vccarousel
<script src='../dist/vc-carousel.js'></script>
```

## Usage

## props

### okText

custom the ok carousel text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel carousel text.

* default: `取消`
* type: `String`

### visiable

control the visiable of carousel.

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
        vccarousel
    } from '../dist/vc-carousel.js'

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
        vccarousel
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
<vc-carousel 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-carousel>
```
