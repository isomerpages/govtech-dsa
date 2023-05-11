---
title: FAQ
permalink: /faq/
---
<style>
ul.accordion {position: relative; margin: 1.4rem 0!important; border-bottom: 1px solid rgba(0,0,0,0.25); padding-bottom: 0;}
ul.accordion li {border-top: 1px solid rgba(0,0,0,0.25); list-style: none; margin-left: 0;}
ul.accordion li input {display: none;}
ul.accordion li label {display: block; cursor: pointer; padding: 0.75rem 2.4rem 0.75rem 0; margin: 0;}
ul.accordion li div {display: none; padding-bottom: 1.2rem;}
ul.accordion li input:checked + label {font-weight: bold;}
ul.accordion li input:checked + label + div {display: block;}
ul.accordion li label::before {content: "+"; font-weight: normal; font-size: 130%; line-height: 1.1rem; padding: 0; position: absolute; right: 0.5rem; transition: all 0.15s ease-in-out;}
ul.accordion li input:checked + label::before {transform: rotate(-45deg);}
</style>

<ul class="accordion">
  <li>
		  <input type="checkbox" id="accordion1">
		  <label for="accordion1">Label 1</label>
		  <div>
				Message Hello Content 2
		  </div>
	</li>
  <li>
		  <input type="checkbox" id="accordion2">
		  <label for="accordion2">Label 2</label>
		  <div>
				Message Hello Content 2
		  </div>
	</li>
  <li>
		  <input type="checkbox" id="accordion3">
		  <label for="accordion3">Label 3</label>
		  <div>
				Message Hello Content 3
		  </div>
	</li>
</ul>