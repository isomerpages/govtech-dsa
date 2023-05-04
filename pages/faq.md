---
title: FAQ
permalink: /faq/
---
<style type="text/css">
$midnight: #2c3e50;
$clouds: #ecf0f1;
/* Accordion styles */
.tabs {
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 4px -2px rgba(0,0,0,0.5);
}
.tab {
  width: 100%;
  color: white;
  overflow: hidden;
  &-label {
    display: flex;
    justify-content: space-between;
    padding: 1em;
    background: $midnight;
    font-weight: bold;
    cursor: pointer;
    /* Icon */
    &:hover {
      background: darken($midnight, 10%);
    }
    &::after {
      content: "\276F";
      width: 1em;
      height: 1em;
      text-align: center;
      transition: all .35s;
    }
  }
  &-content {
    max-height: 0;
    padding: 0 1em;
    color: $midnight;
    background: white;
    transition: all .35s;
  }
  &-close {
    display: flex;
    justify-content: flex-end;
    padding: 1em;
    font-size: 0.75em;
    background: $midnight;
    cursor: pointer;
    &:hover {
      background: darken($midnight, 10%);
    }
  }
}

// :checked
input:checked {
  + .tab-label {
    background: darken($midnight, 10%);
    &::after {
      transform: rotate(90deg);
    }
  }
  ~ .tab-content {
    max-height: 100vh;
    padding: 1em;
  }
}
	</style>

<div class="tabs">
		<div class="tab">
			<input id="chck1" type="checkbox">
			<label for="chck1" class="tab-label">Item 1</label>
			<div class="tab-content">
				Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ipsum, reiciendis!
			</div>
		</div>
		<div class="tab">
			<input id="chck2" type="checkbox">
			<label for="chck2" class="tab-label">Item 2</label>
			<div class="tab-content">
				Lorem ipsum dolor sit amet consectetur adipisicing elit. A, in!
			</div>
		</div>
	</div>