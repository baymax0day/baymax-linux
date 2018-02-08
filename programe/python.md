# Python元素

	1.dict是一个字典,key和value对应 {'key':'value'}
	2.list 相当于个数组 ['a','b','c']

#json操作
	
	1.json.dumps 将Python对象转换为json对象,type是一个字符串str
	2.json.loads 将一个json对象转换成一个Python对象,type是一个list或是dict

# 异常处理

	1.出错即可看到错误信息
	try:
		执行的语句
		=================
	except [异常名称]:
		执行语句
		=================
	else:
		执行语句, 如果没有异常,接着 这里运行
		=================
	例:
		try:
    		fh = open("testfile", "w")
    		fh.write("这是一个测试文件，用于测试异常!!")
		except IOError:
    		print "Error: 没有找到文件或读取文件失败"
		else:
    		print "内容写入文件成功"
    		fh.close()
