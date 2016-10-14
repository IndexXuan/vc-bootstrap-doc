---
title: vc-tabs
type: guide
order: 29
---

* [github](https://github.com/iwaimai-bi-fe/vc-tabs)
* [npm](https://www.npmjs.com/package/vc-tabs)
* [download](https://github.com/iwaimai-bi-fe/vc-tabs/archive/master.zip)

## Install

``` npm
npm install vc-tabs --save
```

``` js
import vcTabs from 'vc-tabs' // build version
import vcTabs from 'vc-tabs/src/Tabs.vue' // recommend for *.vue project for small bundle size
const vcTabset = vcTabs.vcTabset
```

``` js 
// commonjs
require('./dist/build.min.js')
```

``` html
// script tag
<script src='dist/build.min.js'></script>
```

## Usage

## props

### id

可传入id,关闭$parent的autoIndex来用外界传入的index做tab的渲染,高级用法，一般无需使用

* type: `String | Number`

### 'header'

tab title

* type: `String`

### disabled

不响应点击事件，达到不会切换tab的disabled效果

* type: `Boolean`
* default: `false`

`Tabset props`

### name

* type: `String`

### removeable
    
* type: `Boolean`
* default: `false`

### trigger

* type: `String`
* default: `'click'`

### delay

* type: `Number | String`
* default: `120`

### effect

* type: `String`
* default: `'fadein'`

### active

* type: `Number | String`
* default: `0`

### autoIndex

* type: `Boolean`
* default: `true`

## example

* js

```js
import Vue from 'vue'
import { vcTab, vcTabset } from '../src'

new Vue({
    el: '#app',
    data () {
        return {
            active: 0,
            trigger: 'hover',
            autoIndex: true,
            renderData: null,
            header0: 'header0',
            header1: 'header1',
            header2: 'header2'
        }
    },
    ready () {
        this.renderData = this.$refs.tabs.renderData
    },
    methods: {
        deleteTheTab () {
            this.renderData.splice(0, 1)
        }
    },
    components: {
        vcTab,
        vcTabset
    }
})
```

```html
<vc-tabset 
    v-ref:tabs
    :trigger="trigger"
    :active="active"
    :removeable="true"
    :auto-index="autoIndex"
>
    <vc-tab
        :header="header0"
    >
        <div>content0</div>
    </vc-tab>
    <vc-tab
        :header="header1"
    >
        <div>content1</div>
    </vc-tab>
    <vc-tab
        :header="header2"
    >
        <div>content2</div>
    </vc-tab>
    <vc-tab
        :header="header0"
    >
        <div>content0</div>
    </vc-tab>
</vc-tabset>
```
