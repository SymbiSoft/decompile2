作者：中文吊好听

联系方式：include3560@sina.com
声明：允许修改，但必须保留doc信息和写在pyc开法的信息。转载必须标明来源(wap.wapele.cn)
注：只支持大部分的语法…
用法：
import decompile2
try:

> decompile2.main(path,target='d:\\1.py')#target为可选参数，如果没给出则以原路径加“_dis”_

except:

> decompile2.writefile()#如遇到反编出错的就把已反的写进文件

> decompile2.f.close()



新增加直接反编code的功能：

用法：

code=compile('print 1','','exec')



import decompile2

try:

> decompile2.main('','',c=code)#前两个参数必须为空字符串

except:

> decompile2.writefile()#如遇到反编出错的就把已反的写进文件

> decompile2.f.seek(0)

> temp=decompile2.f.read()

> decompile2.f.close()

print temp