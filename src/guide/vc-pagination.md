---
title: vc-pagination
type: guide
order: 28
---

* [github](https://github.com/iwaimai-bi-fe/vc-pagination)
* [npm](https://www.npmjs.com/package/vc-pagination)
* [download](https://github.com/iwaimai-bi-fe/vc-pagination/archive/master.zip)

## Install

```npm
npm install vc-pagination --save
```

```html
//global varibale  vcpagination
<script src='../dist/vc-pagination.js'></script>
```

## Usage

## props

### okText

custom the ok pagination text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel pagination text.

* default: `取消`
* type: `String`

### visiable

control the visiable of pagination.

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
        vcpagination
    } from '../dist/vc-pagination.js'

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
        vcpagination
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
<vc-pagination 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-pagination>
```
