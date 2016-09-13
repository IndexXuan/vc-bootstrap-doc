---
title: vc-spin
type: guide
order: 25
---

* [github](https://github.com/iwaimai-bi-fe/vc-spin)
* [npm](https://www.npmjs.com/package/vc-spin)
* [download](https://github.com/iwaimai-bi-fe/vc-spin/archive/master.zip)

## Install

```npm
npm install vc-spin --save
```

```html
//global varibale  vcspin
<script src='../dist/vc-spin.js'></script>
```

## Usage

## props

### okText

custom the ok spin text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel spin text.

* default: `取消`
* type: `String`

### visiable

control the visiable of spin.

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
        vcspin
    } from '../dist/vc-spin.js'

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
        vcspin
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
<vc-spin 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-spin>
```
