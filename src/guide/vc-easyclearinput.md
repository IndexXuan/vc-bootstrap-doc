---
title: vc-easyclearinput
type: guide
order: 9
---

* [github](https://github.com/iwaimai-bi-fe/vc-easyclearinput)
* [npm](https://www.npmjs.com/package/vc-easyclearinput)
* [download](https://github.com/iwaimai-bi-fe/vc-easyclearinput/archive/master.zip)

## Install

```npm
npm install vc-easyclearinput --save
```

```html
//global varibale  vceasyclearinput
<script src='../dist/vc-easyclearinput.js'></script>
```

## Usage

## props

### okText

custom the ok easyclearinput text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel easyclearinput text.

* default: `取消`
* type: `String`

### visiable

control the visiable of easyclearinput.

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
        vceasyclearinput
    } from '../dist/vc-easyclearinput.js'

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
        vceasyclearinput
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
<vc-easyclearinput 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-easyclearinput>
```
