# resHeaders

修改请求头，配置模式：

	pattern resHeaders://filepath

filepath 为 [Values](http://local.whistlejs.com/#values) 里面的 {key} 或者本地文件(如：`e:\test\xxx`、`e:/test/xxx`、`/User/username/test/xxx` 等):

	x-test1: value1
	x-test2: value2
	x-testN: valueN

pattern 参见[匹配方式](#pattern)，更多模式请参考[配置模式](#mode)，json 格式参考[数据格式](#data)。

例子：

	www.ifeng.com resHeaders://{test-resHeaders.json}


test-resHeaders.json:

	x-test1: value1
	x-test2: value2
	x-testN: valueN
