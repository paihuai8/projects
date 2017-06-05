### 百度动态REM

适应所有移动端设备

```
// 实现所有设备border保持物理1px
// CSS 1px == 设备的物理的1px
var scale = 1 /window.devicePixelRatio 1/2/3
	
	document.write(`
			 <meta name="viewport"
        content="initial-scale=${scale}, maximum-scale=${scale}, minimum-scale=${scale}, user-scalable=no"> 
		`)


	var width = document.documentElement.clientWidth / window.devicePixelRatio
	var scale = width / 375


	// 10rem === 实际页面的宽度
	var css = `
	html{
		font-size:${width / 10 * window.devicePixelRatio}px;
	}
	`
	document.write(`<style>${css}</style>`)
```

### 要点

 - 浏览器禁止980像素的缩放
 - 设置html{font-size:页面宽度 / 10 }px
 - 10rem == 页面宽度
 - 所有单位都用rem === 所有长度都以页面宽度为基准
