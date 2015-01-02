# autoTab [![Build Status](https://travis-ci.org/djhvscf/autoTab.svg?branch=master)](https://travis-ci.org/djhvscf/autoTab)
A plugin that allows the auto tab between inputs and text areas. It is beautiful and lightweight plugin. No jQuery.

Author Homepage:      http://djhvscf.github.io/Blog/<br />

## Current version
* **v1.6.0** `02/Jan/2015`

## Bugs & Enhancements (next version)

## Release history

| Version Number  | Date          |
| --------------- | -----------   |
| v1.6.0		  |	`02/Jan/2015` |
| v1.5.0		  |	`30/Dic/2014` |
| v1.4.2		  |	`29/Dic/2014` |
| v1.4.0		  |	`28/Dic/2014` |
| v1.3.0		  |	`24/Dic/2014` |
| v1.2.0		  |	`24/Dic/2014` |
| v1.0.0		  |	`23/Dic/2014` |

## Dependencies
* In this moment this plugin doesn't have dependencies

## How to Use
Define the property `data-tab` in the input element setting a number between 0 to N like `data-tab="0"` and declare `data-length` in the input element setting a number between 1 to N like `data-length="1"`
this property will be the `maxlength` property in each input element and it helps to plugin knows when change the focus.

**Syntax Example**  
```html
<script src="autoTab.min.js"></script>

<input name="first" id="first" type="text" data-tab="0" data-length="2">
<input name="second" id="second" type="text" data-tab="1" data-length="2">
```
```javascript
(function() {
	// Calling the plugin
	var autoTab = new autoTab();
})();
```

**Parameters**   

| Parameter | Description | Default |
| ----------| ----------- | ------- |
| `autoFocus` | True if you want that the element with `data-tab="0"` has the focus, otherwise, false | `false` |
| `addStyle`  | True if you want to apply the default style of inputs and textareas, otherwise, false | `false` |
| `onComplete` | True if you want to call a function when all the inputs are already "tab-ed", you have to pass the callback function in this parameter | `empty` |
| `onChanged` | Returns a callback with the `event`, it has the information where you can access to key pressed | `empty` |
| `recursive` | True if you want that once the inputs are filled, the plugin start again, otherwise, false | `false` |



**Methods**

| Method | Description |
| ----------| ----------- |
| `destroy` | If you call this method the plugin will be delete and all the styles and events associated with it |

**Demo:** [http://djhvscf.github.io/Blog/experiments/2014/12/autoTab.html](http://djhvscf.github.io/Blog/experiments/2014/12/autoTab.html)

## Reporting issues
Your feedback is very appreciated! <br />
Use this page to report issues (https://github.com/djhvscf/autoTab/issues)