---
title: vc-dropdown
type: guide
order: 11
---

* [github](https://github.com/iwaimai-bi-fe/vc-dropdown)
* [npm](https://www.npmjs.com/package/vc-dropdown)
* [download](https://github.com/iwaimai-bi-fe/vc-dropdown/archive/master.zip)

## Install

```npm
npm install vc-dropdown --save
```

```html
//global varibale  vcdropdown
<script src='../dist/vc-dropdown.js'></script>
```

## Usage

## props

### okText

custom the ok dropdown text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel dropdown text.

* default: `取消`
* type: `String`

### visiable

control the visiable of dropdown.

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
        vcdropdown
    } from '../dist/vc-dropdown.js'

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
        vcdropdown
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
<vc-dropdown 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-dropdown>
```
