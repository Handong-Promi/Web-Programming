Borders
=======

<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
<!-- code_chunk_output -->

- [Border Properties](#border-properties)
- [Border Style](#border-style)
- [Border Width](#border-width)
- [Boarder Color](#boarder-color)
- [Border Sides](#border-sides)
- [Border Shorthand](#border-shorthand)
- [Rounded Borders](#rounded-borders)

<!-- /code_chunk_output -->

---

> 시작 전, 이 문서는 w3schools의 [HTML Block & Inline Elements](https://www.w3schools.com/html/html_blocks.asp)을 참고하였음을 밝힙니다.

---

## Border Properties

CSS `border` 속성을 통해 **element border의 스타일, 너비, 색깔 등을 설정**할 수 있습니다.

***

## Border Style

`border-style` 속성을 통해 **어떤 종류의 border을 화면에 표시**할 것인지 설정할 수 있습니다.

-	종류

	-	`dotted`: Defines a dotted border
	-	`dashed`: Defines a dashed border
	-	`solid`: Defines a solid border
	-	`double`: Defines a double border
	-	`groove`: Defines a 3D grooved border. The effect depends on the border-color value
	-	`ridge`: Defines a 3D ridged border. The effect depends on the border-color value
	-	`inset`: Defines a 3D inset border. The effect depends on the border-color value
	-	`outset`: Defines a 3D outset border. The effect depends on the border-color value
	-	`none`: Defines no border
	-	`hidden`: Defines a hidden border

		[(출처: w3schools CSS Border Style)](https://www.w3schools.com/css/css_border.asp)

`border-style` 속성은 **한 개에서 네 개까지의 값**을 가질 수 있습니다. (상하좌우)

-	예시

	```html
	<!DOCTYPE html>
	<html>
	<head>
	<style>
		p.dotted {border-style: dotted;}
		p.dashed {border-style: dashed;}
		p.solid {border-style: solid;}
		p.double {border-style: double;}
		p.groove {border-style: groove;}
		p.ridge {border-style: ridge;}
		p.inset {border-style: inset;}
		p.outset {border-style: outset;}
		p.none {border-style: none;}
		p.hidden {border-style: hidden;}
		p.mix {border-style: dotted dashed solid double;}
	</style>
	</head>
	<body>

		<h2>The border-style Property</h2>
		<p>This property specifies what kind of border to display:</p>

		<p class="dotted">A dotted border.</p>
		<p class="dashed">A dashed border.</p>
		<p class="solid">A solid border.</p>
		<p class="double">A double border.</p>
		<p class="groove">A groove border.</p>
		<p class="ridge">A ridge border.</p>
		<p class="inset">An inset border.</p>
		<p class="outset">An outset border.</p>
		<p class="none">No border.</p>
		<p class="hidden">A hidden border.</p>
		<p class="mix">A mixed border.</p>


	</body>
	</html>
	```
	![border-style](https://i.imgur.com/IuXJwYw.png)

	> `border-style`이 설정되어 있어야 Width, Color 등의 속성을 border에 적용할 수 있으니 주의하도록 합시다. (if not, 속성 적용 안됨. 화면에 표시 안됨.)

***

## Border Width

`border-width` 속성은 네 가장자리의 폭(너비)를 지정합니다.

- __width 지정 방법__

	1. 특정 단위 사용
		- px
		- pt
		- cm
		- em

	2. 미리 정의된 값 사용
		- thin
		- medium
		- thick

- `border-style`과 마찬가지로 상하좌우 가장자리에 대한 각각의 값을 지정할 수 있습니다.

- 여러 차례의 실험 결과, border-style만 적용했을 때의 **border-width의 default값은 3px**이다.

- 예시
	```html
	<!DOCTYPE html>
	<html>
	<head>
	<style>
		p.one {
		  border-style: solid;
		  border-width: 5px;
		}

		p.two {
		  border-style: solid;
		  border-width: medium;
		}

		p.three {
		  border-style: solid;
		  border-width: 25px 10px 4px 35px;
		}
	</style>
	</head>
	<body>

		<p class="one">Some text.</p>
		<p class="two">Some text.</p>
		<p class="three">Some text.</p>

	</body>
	</html>
	```
	![border-width](https://i.imgur.com/AR9EBRr.png)

***

## Boarder Color

`border-color` 속성은 네 가장자리의 색을 지정합니다.

- 가능한 설정
	- name: specify a color name, like "red"
	- HEX: specify a HEX value, like "#ff0000"
	- RGB: specify a RGB value, like "rgb(255,0,0)"
	- HSL: specify a HSL value, like "hsl(0, 100%, 50%)"
	- transparent   

		[(출처: w3schools CSS Border Color)](https://www.w3schools.com/css/css_border_color.asp)

- 만약 `border-color` 속성이 설정되어있지 않다면, 해당 element의 속성을 상속받습니다.

- 예시
	```html
	<!DOCTYPE html>
	<html>
	<head>
	<style>
		p.one {
		  border-style: solid;
		  border-color: red;
		}

		p.two {
		  border-style: dotted;
		  border-color: green;
		}

		p.three {
	  	  border-style: solid;
    	  border-color: red green blue yellow;
		}
	</style>
	</head>
	<body>

		<p class="one">A solid red border</p>
		<p class="two">A dotted green border</p>
		<p class="three">A solid multicolor border</p>

	</body>
	</html>
	```
	![border-color](https://i.imgur.com/lERszI4.png)

***

## Border Sides

`border-___-style` 속성을 통해, Border 상하좌우 가장자리 각각을 따로 스타일링 할 수 있습니다.

- 종류
	- `border-top-style`
	- `border-right-style`
	- `border-bottom-style`
	- `border-left-style`

- 만약 `border-style` 속성값으로 하나가 아닌 2~4개의 값이 왔을 때
	- 2개: top & bottom / right & left 적용
	- 3개 : top / right & left / bottom 적용
	- 4개 : top / right / bottom / left
		> 순서에 !유의!합시다.

- 예시
	```html
	<!DOCTYPE html>
	<html>
	<head>
	<style>
		p {
		  border-style: dotted solid;
		}
	</style>
	</head>
	<body>

		<p>2 different border styles.</p>

	</body>
	</html>
	```

	![Individual-border](https://i.imgur.com/kmxK0UI.png)

***

## Border Shorthand

`border-width`, `border-style`, `border-color` 이 세 가지 속성을 `border` 속성으로 한 번에 표현할 수 있습니다.

- `border: width style color`. // 순서를 기억하자!

- `border-top`, `border-bottom`, `border-right`, `border-left`로 각각의 가장자리만 따로 border 스타일링을 할 수 있습니다.

- 예시

	```html
	<!DOCTYPE html>
	<html>
	<head>
	<style>
	  p.one {
	    border: 5px solid red;
	  }
	  p.two {
	    border-left: 6px solid red;
	    background-color: lightgrey;
	  }
	</style>
	</head>
	<body>

	  <p class="one">This property is a shorthand property for border-width, border-style, and border-color.</p>
	  <p class="two">This property is a shorthand property for border-left-width, border-left-style, and border-left-color.<p>
	</body>
	</html>
	```
	![border-shorthand](https://i.imgur.com/jmaTa3e.png)

***

## Rounded Borders

`border-radius` 속성을 통해 element의 가장자리를 둥그렇게 만들 수 있습니다.

- 예시

	```html
	<!DOCTYPE html>
	<html>
	<head>
	<style>
	  p.normal {
	    border: 2px solid red;
	  }

	  p.round1 {
	    border: 2px solid red;
	    border-radius: 5px;
	  }

	  p.round2 {
	    border: 2px solid red;
	    border-radius: 8px;
	  }

	  p.round3 {
	    border: 2px solid red;
	    border-radius: 12px;
	  }
	</style>
	</head>
	<body>

	  <p class="normal">Normal border</p>
	  <p class="round1">Round border</p>
	  <p class="round2">Rounder border</p>
	  <p class="round3">Roundest border</p>

	</body>
	</html>
	```
	![rounded-border](https://i.imgur.com/1dTQXt9.png)
