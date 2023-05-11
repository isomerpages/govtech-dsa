---
title: FAQ
permalink: /faq/
---
<style>
ul.jekyllcodex\_accordion {position: relative; margin: 1.4rem 0!important; border-bottom: 1px solid rgba(0,0,0,0.25); padding-bottom: 0;}
ul.jekyllcodex\_accordion li {border-top: 1px solid rgba(0,0,0,0.25); list-style: none; margin-left: 0;}
ul.jekyllcodex\_accordion li input {display: none;}
ul.jekyllcodex\_accordion li label {display: block; cursor: pointer; padding: 0.75rem 2.4rem 0.75rem 0; margin: 0;}
ul.jekyllcodex\_accordion li div {display: none; padding-bottom: 1.2rem;}
ul.jekyllcodex\_accordion li input:checked + label {font-weight: bold;}
ul.jekyllcodex\_accordion li input:checked + label + div {display: block;}
ul.jekyllcodex\_accordion li label::before {content: "+"; font-weight: normal; font-size: 130%; line-height: 1.1rem; padding: 0; position: absolute; right: 0.5rem; transition: all 0.15s ease-in-out;}
ul.jekyllcodex\_accordion li input:checked + label::before {transform: rotate(-45deg);}
</style>

<ul class="jekyllcodex\_accordion">
    {% for item in page.accordion %}
        <li><input type="checkbox" id="accordion{{ forloop.index }}"><label for="accordion{{ forloop.index }}">{{ item.title }}</label><div>{{ item.content | markdownify }}</div></li>
    {% endfor %}
</ul>

---
accordion: 
  - title: this is item 1
    content: Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
  - title: this is item 2
    content: Lorem ipsum dolor sit amet, consectetur adipiscing elit.
---