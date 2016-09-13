---
title: vc-card
type: guide
order: 14
---

* [github](https://github.com/iwaimai-bi-fe/vc-card)
* [npm](https://www.npmjs.com/package/vc-card)
* [download](https://github.com/iwaimai-bi-fe/vc-card/archive/master.zip)

## Install

```npm
npm install vc-card --save
```

```html
//global varibale  vccard
<script src='../dist/vc-card.js'></script>
```

## Usage

## props

### okText

custom the ok card text.

* default: `确定`
* type: `String`

### cancelText

custom the cancel card text.

* default: `取消`
* type: `String`

### visiable

control the visiable of card.

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
        vccard
    } from '../dist/vc-card.js'

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
        vccard
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
<vc-card 
    :visible='isShow'
    :okText='okText'
    :cancelText='cancelText'
    :onOk='onOk'
    :onCancel='onCancel'>
    <div class="your-html">
        
    </div>     
</vc-card>
```
