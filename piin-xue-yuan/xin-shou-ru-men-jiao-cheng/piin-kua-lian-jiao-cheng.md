# Piin跨链教程

若视频没有立即显示，请稍等片刻，等待视频完成加载；

点击视频右上角的“…”，弹出的“download”选项可以将视频下载到本地；

```markdown
<iframe src="https://piin-wiki.github.io/piin-wiki/Piin-cross-chain.html" frameborder="0" width="100%" height="500px" allowfullscreen></iframe>
```

```javascript
// 创建一个新的iframe元素
var iframe = document.createElement('iframe');

// 设置iframe的属性
iframe.src = 'https://piin-wiki.github.io/piin-wiki/Piin-cross-chain.html';
iframe.width = '100%';
iframe.height = '720';
iframe.frameBorder = '0';
iframe.allowFullscreen = true;

// 将allowfullscreen属性转换为布尔值（如果需要）
iframe.allowFullscreen = (iframe.allowFullscreen === 'true');

// 将iframe添加到页面的某个元素中，这里以body为例
document.body.appendChild(iframe);
```

