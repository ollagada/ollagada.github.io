---
layout: page
permalink: /reading-note/
name: Book Review
---

책을 많이 읽고 싶다는 욕구가 생긴만큼
아예 독서 페이지를 제대로 담아둬
책 포스팅만 따로 담아둘 수 있도록 만들었다.

어떤 책인지 한 눈에 담기는 것은 물론,
내 스스로도 책을 더더욱 읽어내고 싶어하는 마음을 주지 않을까

요즘들어 다독이 땡긴다.

현재 읽은 양 : {{site.categories['Book'].size}}

<progress value="{{site.categories['Book'].size}}" max="100"></progress>


<div class="wrapper-reading-note">
    <ul class="book-list">
            {% for post in site.posts %}
                {% if post.category contains 'Book' %}
               <li><a href="{{ post.url | prepand : site.baseurl}}"> {{ post.title }} </a></li>
                {% endif%}
            {% endfor %}
    </ul>
</div>
     