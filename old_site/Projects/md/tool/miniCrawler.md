#MiniCrawler

##Github Path :
<a href ="https://github.com/LixinZhang/miniCrowler" >https://github.com/LixinZhang/miniCrowler </a>

##Introduction:
* MiniCrawler is a simple web crawler implemented by Python.
* Threadpool tech is used to speed up fetching pages.

* One can config the crawler through modify the file <code>config.py</code>.
And start the crawling job using <code>python run.py</code>.
* The webs pages fetched will be stored in <code>pages</code> folder.
* <code>check_status.py</code> helps you check the job's status as following:

<pre>
Rank			Hostname		Times	
----------------------------------------
   1	         buaa.edu.cn	    40	
   2	         baixing.com	    32	
   3	         cnblogs.com	    29	
   4	          hao123.com	     5	
   5	       xinhuanet.com	     2	
   6	      visionplaza.cn	     2	
   7	       people.com.cn	     2	
   8	              org.cn	     2	
   9	             news.cn	     2	
  10	         most.gov.cn	     2
</pre>

##More Detail
You can find more detail in my Chinese Blog. <a href="http://www.cnblogs.com/coser/archive/2012/03/16/2402389.html">Python 多线程抓取网页 </a>
