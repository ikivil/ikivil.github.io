---
layout: post
title:  "添加评论 to Jekyll! "
date:   2016-09-19 10:13:13 +0800
categories: jekyll update
---
## jekyll 添加 `多说` 
jekyll 添加 `多说`  
:one: 编辑 `_config.yml` 添加  
````
# Comment setting
comments :
  provider : duoshuo
  duoshuo :
    short_name : freehyan
```` 

:two: 编辑 `_layouts/post.html` 添加

```html
<!-- 多说评论框 start -->
<div class="ds-thread" data-thread-key="{{ page.id }}" data-title="{{ page.title }}" data-url="{{page.url}}"></div>
<!-- 多说评论框 end -->
<!-- 多说公共JS代码 start (一个网页只需插入一次) -->
<script type="text/javascript">
var duoshuoQuery = {short_name:"ikivil"};
	(function() {
		var ds = document.createElement('script');
		ds.type = 'text/javascript';ds.async = true;
		ds.src = (document.location.protocol == 'https:' ? 'https:' : 'http:') + '//static.duoshuo.com/embed.js';
		ds.charset = 'UTF-8';
		(document.getElementsByTagName('head')[0] 
		 || document.getElementsByTagName('body')[0]).appendChild(ds);
	})();
	</script>
<!-- 多说公共JS代码 end -->
````

{% highlight ruby %}
jekyll serve
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
