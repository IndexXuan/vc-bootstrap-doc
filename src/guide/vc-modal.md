---
title: vc-modal
type: guide
order: 18
---

* [github](https://github.com/iwaimai-bi-fe/vc-modal)
* [npm](https://www.npmjs.com/package/vc-modal)
* [download](https://github.com/iwaimai-bi-fe/vc-modal/archive/master.zip)

## Install

```npm
npm install vc-modal --save
```

```html
//global varibale  vcmodal
<script src='../dist/vc-modal.js'></script>
```

## Usage

## props

### okText

custom the ok modal text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel modal text.

* default: `取消`
* type: `String`

### visiable

control the visiable of modal.

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
        vcmodal
    } from '../dist/vc-modal.js'

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
        vcmodal
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
<vc-modal 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-modal>
```
