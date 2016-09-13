---
title: vc-tooltip
type: guide
order: 22
---

* [github](https://github.com/iwaimai-bi-fe/vc-tooltip)
* [npm](https://www.npmjs.com/package/vc-tooltip)
* [download](https://github.com/iwaimai-bi-fe/vc-tooltip/archive/master.zip)

## Install

```npm
npm install vc-tooltip --save
```

```html
//global varibale  vctooltip
<script src='../dist/vc-tooltip.js'></script>
```

## Usage

## props

### okText

custom the ok tooltip text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel tooltip text.

* default: `取消`
* type: `String`

### visiable

control the visiable of tooltip.

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
        vctooltip
    } from '../dist/vc-tooltip.js'

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
        vctooltip
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
<vc-tooltip 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-tooltip>
```
