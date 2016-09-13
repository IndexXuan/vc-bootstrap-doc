---
title: vc-autocomplete
type: guide
order: 10
---

* [github](https://github.com/iwaimai-bi-fe/vc-autocomplete)
* [npm](https://www.npmjs.com/package/vc-autocomplete)
* [download](https://github.com/iwaimai-bi-fe/vc-autocomplete/archive/master.zip)

## Install

```npm
npm install vc-autocomplete --save
```

```html
//global varibale  vcautocomplete
<script src='../dist/vc-autocomplete.js'></script>
```

## Usage

## props

### okText

custom the ok autocomplete text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel autocomplete text.

* default: `取消`
* type: `String`

### visiable

control the visiable of autocomplete.

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
        vcautocomplete
    } from '../dist/vc-autocomplete.js'

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
        vcautocomplete
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
<vc-autocomplete 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-autocomplete>
```
