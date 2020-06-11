vue-element-spy
========

Plugin for detecting when element reaches top of the viewport. The plugin uses Intersection Observer.

# Installation

```
yarn add vue-element-spy
```

## Import

```javascript
import Vue from 'vue'
import VueElementSpy from 'vue-element-spy'

Vue.use(VueElementSpy)
```

## Browser

```html
<script src="vue.js"></script>
<script src="/node_modules/vue-element-spy/dist/vue-element-spy.js"></script>
```

```javascript
Vue.use(VueElementSpy)
```

## Install options

### refreshInterval

It's possible to set `refreshInterval` option for periodical spies refresh. Use if content changes or reflows without scrolling.
**Default**: `250`
**Disable**: `0`

```javascript
Vue.use(VueElementSpy, {refreshInterval: 500})
```

# Usage

## v-vue-element-spy directive

`v-vue-element-spy` observes whether the target element is at the top of the viewport and calls `callback`.

```html
<div v-vue-element-spy="{callback: myCallback}">
<!-- or shortened syntax -->
<div v-vue-element-spy="myCallback">
```

### v-vue-element-spy options

greedy: true,
offset: 0
outOfContext
