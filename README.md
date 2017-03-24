#gotodate
##gotodate是什么?
可以获取某天，前N天，后N天，当前日期周几，当前日期所在周的周一至周日日期

##使用范例
```javascript
[root@localhost ~]# python
Python 2.7.5 (default, Sep 15 2016, 22:37:39) 
[GCC 4.8.5 20150623 (Red Hat 4.8.5-4)] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> from gotodate.gotodate  import GotoDate
>>> a='2015-10-11'
>>> f=GotoDate(date=a)
>>> f.after(5)
datetime.date(2015, 10, 16)
>>> f.before(4)
datetime.date(2015, 10, 7)
>>> f.week()
6
>>> f.week_range()
{'Monday': datetime.date(2015, 10, 5), 'Tuesday': datetime.date(2015, 10, 6), 'Friday': datetime.date(2015, 10, 9), 'Wednesday': datetime.date(2015, 10, 7), 'Thursday': datetime.date(2015, 10, 8), 'Sunday': datetime.date(2015, 10, 11), 'Saturday': datetime.date(2015, 10, 10)}
>>> 
>>> import datetime
>>> f=GotoDate(date=datetime.datetime.now().date())
>>> f.after(5)
datetime.date(2017, 3, 28)
>>> 

```
##关于作者
chenshancang@163.com