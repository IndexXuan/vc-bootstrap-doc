---
title: vc-tag
type: guide
order: 12
---

* [github](https://github.com/iwaimai-bi-fe/vc-tag)
* [npm](https://www.npmjs.com/package/vc-tag)
* [download](https://github.com/iwaimai-bi-fe/vc-tag/archive/master.zip)

## Install

```npm
npm install vc-tag --save
```

```html
//global varibale  vctag
<script src='../dist/vc-tag.js'></script>
```

## Usage

## props

### okText

custom the ok tag text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel tag text.

* default: `取消`
* type: `String`

### visiable

control the visiable of tag.

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
        vctag
    } from '../dist/vc-tag.js'

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
        vctag
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
<vc-tag 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-tag>
```
