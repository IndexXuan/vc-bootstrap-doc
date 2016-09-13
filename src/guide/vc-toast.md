---
title: vc-toast
type: guide
order: 17
---

* [github](https://github.com/iwaimai-bi-fe/vc-toast)
* [npm](https://www.npmjs.com/package/vc-toast)
* [download](https://github.com/iwaimai-bi-fe/vc-toast/archive/master.zip)

## Install

```npm
npm install vc-toast --save
```

```html
//global varibale  vctoast
<script src='../dist/vc-toast.js'></script>
```

## Usage

## props

### okText

custom the ok toast text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel toast text.

* default: `取消`
* type: `String`

### visiable

control the visiable of toast.

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
        vctoast
    } from '../dist/vc-toast.js'

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
        vctoast
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
<vc-toast 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-toast>
```
