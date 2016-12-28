# jquery-inertiaScroll
慣性スクロールのアニメーション用jQueryプラグイン


## Demo
<a href="http://underground0930.github.io/jquery-inertiaScroll/" target="_blank">demo</a>

##Depends
* jQuery 1.9.1

## Browsers
IE10+ and other new browsers.

## Options
| key  | Value  | initial value |
| :-----  | :----- | :----- |
| parent | body直下のすべてのコンテンツを囲う要素を指定 | none |
| childDelta1 | 少ないと滑らかになる、大きいと進みすぎるので注意 | 0.02 |
| childDelta2 | 子要素のスクロールスピード、大きすぎると滑らかさが無くなる | 0.1 |
| parentDelta | parentのスクロールスピード | 0.08 |

## data Attribute
| key  | Value  | initial value |
| :-----  | :----- | :----- |
| data-speed | 各要素のスクロールスピードを個別に変更出来る | 1 |
| data-margin | 各要素のtranslate3dの値の切片を設定出来る | 0 |


## Usage
```
  <div id="content">
    <header>header!</header>
    <div id="box1" class="box" data-speed="1" data-margin="100"></div>
    <div id="box2" class="box" data-speed="7"></div>
    <div id="box3" class="box" data-speed="2"></div>
    <div id="box4" class="box" data-speed="5"></div>
    <div id="box5" class="box" data-speed="3" data-margin="200"></div>
    <div id="box6" class="box" data-speed="1"></div>
    <div id="box7" class="box" data-speed="2"></div>
    <div id="box8" class="box" data-speed="8"></div>
    <div id="box9" class="box" data-speed="1"></div>
    <div id="box10" class="box" data-speed="5"></div>
    <footer>footer!</footer>
  </div>


	<script>
	$(function(){

	  $(".box").inertiaScroll({
	    parent: $("#content")
	  });

	});  
	</script>


```

## Lisence
Copyright(c) 2016 Go Nishiduka
Licensed under the MIT license.