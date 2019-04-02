# DingDingAppDelete
## 本程序所用的接口仅限企业调用，ISV无法调用
由于钉钉没有提供删除微应用和E应用的按钮，查找文档后发现需要使用工具构建请求，使用本工具即可快速删除不需要的应用。注意：应用删除可能会造成损失，请谨慎操作！

## 开发语言：Python3 使用库：requests/json

## FAQ：访问ip不在白名单之中
当请求开放平台服务端接口遇到此类时，表示您的请求ip不在appkey的服务器出口ip中。按以下方式排查并修改：

1、上开发者后台打开您的应用，这里一定要确认appkey要对应上。

2、点击“修改”，把返回错误接口里的request ip地址加到服务器出口IP列表中。

3、如果遇到明明已经修改了应用的服务器出口IP，但是调用接口还是报错的话。这个时候一定要再次查看下您的代码，确认下appkey和应用是不是一一对应的。



## 钉钉官方文档
### 本程序用的文档，可以直接查看库中的“钉钉删除应用.pdf”文件  

### 获取钉钉应用的access_token
https://open-doc.dingtalk.com/microapp/serverapi2/eev437

### 钉钉官方关于应用管理的文档

https://open-doc.dingtalk.com/doc2/detail.htm?treeId=172&articleId=104978&docType=1#s4
