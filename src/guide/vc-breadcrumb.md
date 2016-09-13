---
title: vc-breadcrumb
type: guide
order: 27
---

* [github](https://github.com/iwaimai-bi-fe/vc-breadcrumb)
* [npm](https://www.npmjs.com/package/vc-breadcrumb)
* [download](https://github.com/iwaimai-bi-fe/vc-breadcrumb/archive/master.zip)

## Install

```npm
npm install vc-breadcrumb --save
```

```html
//global varibale  vcbreadcrumb
<script src='../dist/vc-breadcrumb.js'></script>
```

## Usage

## props

### okText

custom the ok breadcrumb text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel breadcrumb text.

* default: `取消`
* type: `String`

### visiable

control the visiable of breadcrumb.

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
        vcbreadcrumb
    } from '../dist/vc-breadcrumb.js'

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
        vcbreadcrumb
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
<vc-breadcrumb 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-breadcrumb>
```
