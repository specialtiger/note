## node版本

pomelo chat 例子需要降低node版本到5.x

	安装nvm
	curl -o- [https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh](https://link.jianshu.com/?t=https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh) | bash
	nvm install v5.12.0

## 通过修改配置扩充chat服务器

route， dispatch

## 增加filter
	在before filter里，可以做一些请求排队，超时处理, 而在after filter里做一些清理记录的处理。比如，为了统计Handler的处理请求时间，可以在before filter里给session记录一个时间戳，在after filter里取出刚才的时间戳，跟当前时间做运算，就能得到Handler处理请求的时间

## route压缩
	config/dictionary.json映射从1累加
	
## protobuf 
	定义clientProtos.js, serverProtos.js
	useProtobuf:true
	
## 增加rpc服务器
	app.js定义route
	
