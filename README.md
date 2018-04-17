# yj
学习python

for i  in range(26):                    

去掉list中的[]
>>> list = [1,2,3]
>>> str(list).strip('[]')
'1, 2, 3'




from django.urls import * #当你导入的时候找不到


近期计划：流畅的Python



类型是属于对象的

"hi there %s" %（ name，） == "hi is %s"%format(name)#格式化字符串


*********单例模式
在 Python 中，我们可以用多种方法来实现单例模式：

    使用模块
    使用 __new__
    使用装饰器（decorator）
    使用元类（metaclass）


is是对比地址 == 是对比值 # 

redis原理：redis常用的数据类型：string，hash，list，set， sorted set    ；；redis复制机制
持久化方式不够成熟，使用Memcached可能更合适持久

urllib和urllib2的区别

问过,答的urllib2可以Post而urllib不可以.

    urllib提供urlencode方法用来GET查询字符串的产生，而urllib2没有。这是为何urllib常和urllib2一起使用的原因。
    urllib2可以接受一个Request类的实例来设置URL请求的headers，urllib仅可以接受URL。这意味着，你不可以伪装你的User Agent字符串等。


 		Cookie 						Session
储存位置 	客户端 						服务器端
目的 	跟踪会话，也可以保存用户偏好设置或者保存用户名密码等 	跟踪会话
安全性 		不安全 						安全


尝试使用尾递归








Python的标准比较运算符：<、<=、 > 、>=、 ==、 != 、<> 
标准比较运算符对应操作：小于、小于等于、大于、大于等于、等于、不等于、不等于 




unicode转中文
1 >>> s = u'\u4eba\u751f\u82e6\u77ed\uff0cpy\u662f\u5cb8'
2 >>> print s
3 人生苦短，py是岸

1 >>> s = r'\u4eba\u751f\u82e6\u77ed\uff0cpy\u662f\u5cb8'
2 >>> s = s.decode('unicode_escape')
3 >>> print s
4 人生苦短，py是岸

在python2的字符编码问题时常会遇到“UnicodeEncodeError: 'ascii' codec can't encode characters in position 0-5: ordinal not in range(128)”的编码错误。
而用以下方法通常可以解决：

1 import sys
2 reload(sys)
3 sys.setdefaultencoding('utf-8')
此方法是将Python2的默认编码ASCII改为 utf-8。但此方法不是一劳永逸的，可能会使一些代码的行为变得怪异




———————————————————————————————————————————————————————————————————————————————————————————————————————

类的私有属性：self.__name  
在python的实际是(self._Programer__name)直接访问不了加._Programer
python的私有方法其实是障眼法



手动破解pycharm
https://www.cnblogs.com/medivhxu/p/6856756.html
用户名：idea
用户邮箱：idea@163.com


nginx 分布式：
1.将软件各个服务分布在不同的服务器上面，
2.有的数据是在redis上面 ，所以该成直接获取数据库的数据
（其他服务器是访问这台redis，）



python中有一个zfill方法用来给字符串前面补0，非常有用n = "123" s = n.zfill(5)


python 字符串也好，列表也好，都是可迭代对象，比较字符串大小从第一个开始比较第一个谁大就是谁大，相等比二个
有order（），cmp（）


Django查询语句http://www.cnblogs.com/rinka/p/django_make_queries_anout_built-in_lookups.html


SQLserver查询下级部门的sql :https://www.cnblogs.com/adandelion/archive/2007/12/03/981392.html
国外新闻： http://www.ltaaa.com/wtfy/24136.html


后端获取数据
前端拼接数据，前端把数据传到后台


Django的内建标签
block：使用形式：
	{%block%}定义块内容{%endblock%} 
	意义：定义一个块，该块能被继承他的子孙重写


comment：使用形式：
	{%comment%}内容{%endcomment%}
