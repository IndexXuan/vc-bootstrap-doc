---
title: vc-popover
type: guide
order: 21
---

* [github](https://github.com/iwaimai-bi-fe/vc-popover)
* [npm](https://www.npmjs.com/package/vc-popover)
* [download](https://github.com/iwaimai-bi-fe/vc-popover/archive/master.zip)

## Install

```npm
npm install vc-popover --save
```

```html
//global varibale  vcpopover
<script src='../dist/vc-popover.js'></script>
```

## Usage

## props

### okText

custom the ok popover text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel popover text.

* default: `取消`
* type: `String`

### visiable

control the visiable of popover.

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
        vcpopover
    } from '../dist/vc-popover.js'

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
        vcpopover
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
<vc-popover 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-popover>
```
