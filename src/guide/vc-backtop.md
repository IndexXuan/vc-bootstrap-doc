---
title: vc-backtop
type: guide
order: 26
---

* [github](https://github.com/iwaimai-bi-fe/vc-backtop)
* [npm](https://www.npmjs.com/package/vc-backtop)
* [download](https://github.com/iwaimai-bi-fe/vc-backtop/archive/master.zip)

## Install

```npm
npm install vc-backtop --save
```

```html
//global varibale  vcbacktop
<script src='../dist/vc-backtop.js'></script>
```

## Usage

## props

### okText

custom the ok backtop text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel backtop text.

* default: `取消`
* type: `String`

### visiable

control the visiable of backtop.

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
        vcbacktop
    } from '../dist/vc-backtop.js'

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
        vcbacktop
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
<vc-backtop 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-backtop>
```
