---
title: vc-notification
type: guide
order: 20
---

* [github](https://github.com/iwaimai-bi-fe/vc-notification)
* [npm](https://www.npmjs.com/package/vc-notification)
* [download](https://github.com/iwaimai-bi-fe/vc-notification/archive/master.zip)

## Install

```npm
npm install vc-notification --save
```

```html
//global varibale  vcnotification
<script src='../dist/vc-notification.js'></script>
```

## Usage

## props

### okText

custom the ok notification text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel notification text.

* default: `取消`
* type: `String`

### visiable

control the visiable of notification.

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
        vcnotification
    } from '../dist/vc-notification.js'

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
        vcnotification
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
<vc-notification 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-notification>
```
