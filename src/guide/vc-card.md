---
title: vc-card
type: guide
order: 14
---

* [github](https://github.com/iwaimai-bi-fe/vc-card)
* [npm](https://www.npmjs.com/package/vc-card)
* [download](https://github.com/iwaimai-bi-fe/vc-card/archive/master.zip)

## Install


``` npm
npm install vc-card --save
```

``` js
import vcCard from 'vc-card' // build version
import vcCard from 'vc-card/src/Card.vue' // recommend for *.vue project for small bundle size
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

### title 

* type: `String`

### content

* type: `String`,

### bordered

* type: `Boolean`,
* default: `true`

### bodyClass

* type: `String`


## example

* js

```js
import Vue from 'vue'
import vcCard from '../src'

new Vue({
    el: '#app',
    data () {
        return {
            bools: {
                'true': true,
                'false': false
            },
            title: 'title',
            content: 'content',
            bordered: true,
            bodyClass: 'body-class'
        }
    },
    components: {
        vcCard
    }
})
```

```html
<vc-card
    :title="title"
    :content="content"
    :bordered="bordered"
>
    content
</vc-card>
```
