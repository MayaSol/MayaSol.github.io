---
layout: post
title:  "Атрибуты поста или страницы в wordpress"
date:   2019-06-01 19:21:59 +0300
categories: wordpress post page
---

[Как получить slug текущей страницы Wordpress](https://wordpress.stackexchange.com/questions/42117/how-do-i-retrieve-the-slug-of-the-current-page)

Получить атрибуты поста Wordrpess находясь внутри Loop
([Function Reference/$post](https://codex.wordpress.org/Function_Reference/$post))

{% highlight php %}
global $post;
echo $post->post_title;
{% endhighlight %}

Получить атрибуты страницы Wordpress вне Loop

{% highlight php %}
$the_page = sanitize_post( $GLOBALS['wp_the_query']->get_queried_object() );
$slug = $the_page->post_name;
{% endhighlight %}