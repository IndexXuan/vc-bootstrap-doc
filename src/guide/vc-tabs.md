---
title: vc-tabs
type: guide
order: 29
---

* [github](https://github.com/iwaimai-bi-fe/vc-tabs)
* [npm](https://www.npmjs.com/package/vc-tabs)
* [download](https://github.com/iwaimai-bi-fe/vc-tabs/archive/master.zip)

## Install

```npm
npm install vc-tabs --save
```

```html
//global varibale  vctabs
<script src='../dist/vc-tabs.js'></script>
```

## Usage

## props

### okText

custom the ok tabs text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel tabs text.

* default: `取消`
* type: `String`

### visiable

control the visiable of tabs.

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
        vctabs
    } from '../dist/vc-tabs.js'

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
        vctabs
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
<vc-tabs 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-tabs>
```
