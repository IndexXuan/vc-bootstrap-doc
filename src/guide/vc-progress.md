---
title: vc-progress
type: guide
order: 23
---

* [github](https://github.com/iwaimai-bi-fe/vc-progress)
* [npm](https://www.npmjs.com/package/vc-progress)
* [download](https://github.com/iwaimai-bi-fe/vc-progress/archive/master.zip)

## Install

```npm
npm install vc-progress --save
```

```html
//global varibale  vcprogress
<script src='../dist/vc-progress.js'></script>
```

## Usage

## props

### okText

custom the ok progress text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel progress text.

* default: `取消`
* type: `String`

### visiable

control the visiable of progress.

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
        vcprogress
    } from '../dist/vc-progress.js'

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
        vcprogress
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
<vc-progress 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-progress>
```
