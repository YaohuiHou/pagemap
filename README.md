# pagemap

[![license][license-img]][github] [![web][web-img]][web] [![github][github-img]][github] [![npm][npm-img]][npm]  
[![version][npm-v-img]][npm] [![downloads][npm-dm-img]][npm] [![build status][travis-img]][travis]

Mini map for web pages.

## Example usage

## [pagemap.js](https://larsjung.de/pagemap/)
pagemap.js是一款基于canvas的web页面mini导航面板插件。该插件可以为web页面制作出类似sublime编辑器右侧的mini导航面板效果。

[pagemap npm](https://www.npmjs.com/package/pagemap) install

```bash
npm i pagemap
```

html导入

```html
<script type="text/javascript" src="/pagemap.min.js"></script>
```
html添加一个canvas元素，绘制微地图需要。

```html
<canvas id='map'></canvas>
```
CSS样式

```css
#map {
    position: fixed;
    top: 0;
    right: 0;
    width: 200px;
    height: 100%;
    z-index: 100;
}
```
初始化插件

```js
pagemap(document.querySelector('#map'));

// 样式可以修改
pagemap(document.querySelector('#map'), {
	viewport: null,
	styles: {
		'header,footer,section,article': 'rgba(0,0,0,0.08)',
		'h1,a': 'rgba(0,0,0,0.10)',
		'h2,h3,h4': 'rgba(0,0,0,0.08)'
	},
	back: 'rgba(0,0,0,0.02)',
	view: 'rgba(0,0,0,0.05)',
	drag: 'rgba(0,0,0,0.10)',
	interval: null
});
```
