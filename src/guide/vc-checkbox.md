---
title: vc-checkbox
type: guide
order: 8
---

* [github](https://github.com/iwaimai-bi-fe/vc-checkbox)
* [npm](https://www.npmjs.com/package/vc-checkbox)
* [download](https://github.com/iwaimai-bi-fe/vc-checkbox/archive/master.zip)

## Install

```npm
npm install vc-checkbox --save
```

```html
//global varibale  vccheckbox
<script src='../dist/vc-checkbox.js'></script>
```

## Usage

## props

### okText

custom the ok checkbox text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel checkbox text.

* default: `取消`
* type: `String`

### visiable

control the visiable of checkbox.

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
        vccheckbox
    } from '../dist/vc-checkbox.js'

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
        vccheckbox
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
<vc-checkbox 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-checkbox>
```
