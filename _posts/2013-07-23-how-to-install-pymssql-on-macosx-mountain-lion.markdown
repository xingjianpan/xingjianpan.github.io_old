---
layout: post
title: How to install pymssql on Mac OS X Mountain Lion?
date: 2013-07-23 21:16:36
categories: python

---
## Problem
### When trying to install pymssql using pip, I got below error message

		_mssql.c:257:10: fatal error: 'sqlfront.h' file not found 


## Solution

### Pre-requeists:
1. Cython (pip install Cython)
2. FreeTDS
	* Download latest stable release from [here](http://www.freetds.org)
	* do the install
	
	`command`

		./configure --prefix=/usr/local/freetds --enable-msdblib
		make
		make install
3. open setup.py

	
Find 

{% highlight python %}
	if sys.platform == 'darwin':
    	fink = '/sw/'
    	if osp.exists(fink):
        	include_dirs.insert(0, fink + 'include')
        	library_dirs.insert(0, fink + 'lib')

{% endhighlight %}
Change to 
{% highlight python %}	
if sys.platform == 'darwin':
	#fink = '/sw/'
	#if osp.exists(fink):
		#include_dirs.insert(0, fink + 'include')
		#library_dirs.insert(0, fink + 'lib')
{% endhighlight %}

4.still in setup.py
 
look for
{% highlight python %}		
if osp.exists('/opt/local'):
    # some mac ports paths
    include_dirs += [
        '/opt/local/include',
        '/opt/local/include/freetds',
        '/opt/local/freetds/include'
    ]   
    library_dirs += [
        '/opt/local/lib',
        '/opt/local/lib/freetds',
        '/opt/local/freetds/lib'
    ]   
{% endhighlight %}		  

change to
{% highlight python %}	
if osp.exists('/usr/local'):
    # some mac ports paths
    include_dirs += [
        '/usr/local/include',
        '/usr/local/include/freetds',
        '/usr/local/freetds/include'
    ]   
    library_dirs += [
        '/usr/local/lib',
        '/usr/local/lib/freetds',
        '/usr/local/freetds/lib'
    ] 	 
{% endhighlight  %}	   
	
change _opt_ to _usr_ as we installed FreeTDS under /usr/local/freetds


### download pymmsql and install
1. Download pymssql from its official site.
2. Do the install, in pymssql's folder,type

		python setup.py install
3. Done!!


## References
1. [blog](http://blog.sina.com.cn/s/blog_62b2318d0101gucr.html)
2. [Issue Discussion](https://groups.google.com/forum/#!topic/pymssql/Z0HuJpJGAfo)



## Resouces
1. [pymssql](http://code.google.com/p/pymssql/downloads/list)	

## Alternative methods
1. [pymssql-macosx-lion](https://github.com/blackbass1988/pymssql-macos-lion)
