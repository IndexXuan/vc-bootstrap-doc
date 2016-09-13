---
title: vc-buttonGroup
type: guide
order: 6
---

* [github](https://github.com/iwaimai-bi-fe/vc-buttonGroup)
* [npm](https://www.npmjs.com/package/vc-buttonGroup)
* [download](https://github.com/iwaimai-bi-fe/vc-buttonGroup/archive/master.zip)

## Install

```npm
npm install vc-buttonGroup --save
```

```html
//global varibale  vcbuttonGroup
<script src='../dist/vc-buttonGroup.js'></script>
```

## Usage

## props

### okText

custom the ok buttonGroup text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel buttonGroup text.

* default: `取消`
* type: `String`

### visiable

control the visiable of buttonGroup.

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
        vcbuttonGroup
    } from '../dist/vc-buttonGroup.js'

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
        vcbuttonGroup
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
<vc-buttonGroup 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-buttonGroup>
```
