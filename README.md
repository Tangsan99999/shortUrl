# Url-Shorten-Worker
A URL Shortener created using Cloudflare Worker

# Getting start
### 去Workers KV中创建一个命名空间

Go to Workers KV and create a namespace.

<img src="https://cdn.jsdelivr.net/npm/imst@0.0.4/20201205232805.png">

### 去Worker的Settings选选项卡中绑定KV Namespace

Bind an instance of a KV Namespace to access its data in a Worker.

<img src="https://cdn.jsdelivr.net/npm/imst@0.0.4/20201205232536.png">

### 其中Variable name填写`LINKS`, KV namespace填写你刚刚创建的命名空间

Where Variable name should set as `LINKS` and KV namespace is the namespace you just created in the first step.

<img src="https://cdn.jsdelivr.net/npm/imst@0.0.4/20201205232704.png">

### 复制本项目中的`index.js`的代码到Cloudflare Worker 

Copy the `index.js` code from this project to Cloudflare Worker. 

### 点击Save and Deploy

Click Save and Deploy

# Demo
https://020.name
 
Note: Because someone abuse this demo website, all the generated link may be deleted at any time. For long-term use, please deploy your own.

注意：由于该示例服务被人滥用，用于转发诈骗网站，故所有由demo网站生成的链接随时可能失效，如需长期使用请自行搭建。

## 感谢
项目基于[xyTom/Url-Shorten-Worker](https://github.com/xyTom/Url-Shorten-Worker)[(MIT)](https://github.com/xyTom/Url-Shorten-Worker/blob/main/LICENSE)  
1. 改进了正则匹配，
1. 添加了超时判断处理，
1. 添加了白名单支持，

