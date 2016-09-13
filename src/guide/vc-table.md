---
title: vc-table
type: guide
order: 24
---

* [github](https://github.com/iwaimai-bi-fe/vc-table)
* [npm](https://www.npmjs.com/package/vc-table)
* [download](https://github.com/iwaimai-bi-fe/vc-table/archive/master.zip)

## Install

```npm
npm install vc-table --save
```

```html
//global varibale  vctable
<script src='../dist/vc-table.js'></script>
```

## Usage

## props

### okText

custom the ok table text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel table text.

* default: `取消`
* type: `String`

### visiable

control the visiable of table.

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
        vctable
    } from '../dist/vc-table.js'

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
        vctable
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
<vc-table 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-table>
```
