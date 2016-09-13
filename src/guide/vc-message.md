---
title: vc-message
type: guide
order: 16
---

* [github](https://github.com/iwaimai-bi-fe/vc-message)
* [npm](https://www.npmjs.com/package/vc-message)
* [download](https://github.com/iwaimai-bi-fe/vc-message/archive/master.zip)

## Install

```npm
npm install vc-message --save
```

```html
//global varibale  vcmessage
<script src='../dist/vc-message.js'></script>
```

## Usage

## props

### okText

custom the ok message text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel message text.

* default: `取消`
* type: `String`

### visiable

control the visiable of message.

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
        vcmessage
    } from '../dist/vc-message.js'

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
        vcmessage
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
<vc-message 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-message>
```
