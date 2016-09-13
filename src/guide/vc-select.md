---
title: vc-select
type: guide
order: 4
---

* [github](https://github.com/iwaimai-bi-fe/vc-select)
* [npm](https://www.npmjs.com/package/vc-select)
* [download](https://github.com/iwaimai-bi-fe/vc-select/archive/master.zip)

## Install

```npm
npm install vc-select --save
```

```html
//global varibale  vcselect
<script src='../dist/vc-select.js'></script>
```

## Usage

## props

### okText

custom the ok select text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel select text.

* default: `取消`
* type: `String`

### visiable

control the visiable of select.

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
        vcselect
    } from '../dist/vc-select.js'

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
        vcselect
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
<vc-select 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-select>
```
