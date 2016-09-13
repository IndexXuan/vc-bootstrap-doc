---
title: vc-alert
type: guide
order: 13
---

* [github](https://github.com/iwaimai-bi-fe/vc-alert)
* [npm](https://www.npmjs.com/package/vc-alert)
* [download](https://github.com/iwaimai-bi-fe/vc-alert/archive/master.zip)

## Install

```npm
npm install vc-alert --save
```

```html
//global varibale  vcalert
<script src='../dist/vc-alert.js'></script>
```

## Usage

## props

### okText

custom the ok alert text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel alert text.

* default: `取消`
* type: `String`

### visiable

control the visiable of alert.

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
        vcalert
    } from '../dist/vc-alert.js'

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
        vcalert
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
<vc-alert 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-alert>
```
