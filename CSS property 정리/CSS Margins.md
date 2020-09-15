Margins
=======
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
<!-- code_chunk_output -->

- [Margins](#margins)
- [Margin - Individual Sides](#margin-individual-sides)
- [Margin - Shorthand Property](#margin-shorthand-property)
- [The auto Value](#the-auto-value)
- [The inherit value](#the-inherit-value)

<!-- /code_chunk_output -->

---

> 시작 전, 이 문서는 w3schools의 [CSS Margins](https://www.w3schools.com/css/css_margin.asp)을 참고하였음을 밝힙니다.

---

## Margins

CSS의 `margin` 속성을 이용하여, element 주변 및 명시 border들의 바깥쪽 공간을 만들어낼 수 있습니다.

- **Element 바깥 공간을 다루는** CSS 속성이라고 생각하면 됩니다.
- top / right / bottom / left에 있어서 각각의 세팅이 가능합니다.

****

## Margin - Individual Sides

1. CSS에서는 한 element의 각 측면에 대한 margin 조정이 가능합니다.

- `margin-top`
- `margin-right`
- `margin-bottom`
- `margin-left`

2. 모든 margin 속성에는 다음과 같은 값들이 올 수 있습니다.
- **auto**: 브라우저가 margin을 자동으로 계산해줍니다.
- **length**: px, pt, cm 등의 단위로 margin을 직접 지정합니다.
- **%**: 포함하고 있는 element의 width를 기준으로, 몇 퍼센트를 margin으로 삼을 것인지 지정할 수 있습니다.
- **inherit**: 부모 element로부터 margin 값을 받도록 지정할 수 있습니다.

3. length와 %에 있어서, **Negative 값도 가능**합니다.

4. 예시
	```html
	<!DOCTYPE html>
	<html>
	<head>
	<style>
		div {
		border: 1px solid black;
	  	margin-top: 100px;
	  	margin-bottom: 100px;
	  	margin-right: 150px;
	  	margin-left: 80px;
		background-color:lightblue;
		}
	</style>
	</head>
	<body>
		<div>이 div element는 top margin을 100px로, right margin을 150px로, bottom margin을 100px로, left margin을 80px로 갖습니다.</div>
	</body>
	</html>
	```
	![margin](https://i.imgur.com/iv4tOl9.png)   
	![margin-develop](https://i.imgur.com/l6ovzk4.jpg)

***

## Margin - Shorthand Property
`margin` 속성을 통해 `margin-top`, `margin-right`, `margin-bottom`, `margin-left` 네 개의 속성을 한 번에 표현할 수 있습니다.
- `margin`의 속성값이 몇 개인지에 따라, 상하좌우 각각에 어떻게 적용되는지 달라집니다.
	- 1개 : Every side
	- 2개: top & bottm / right & left
	- 3개 : top / right & left / bottom
	- 4새 : top / right / bottom / left

***

## The auto Value

margin 속성을 `auto`로 설정함으로써, element를 (자신이 포함된) **container 내에서 수평으로 중앙에 배치할 수 있습니다.**

- `margin` 속성값을 `auto`로 가진 element는 **지정된 너비를 차지**하고, 그런 후 **남은 공간은 좌우 margin 사이에 균등하게 분할**됩니다.
- 실험결과, `auto` 속성값은 `margin`에 적용시 좌우 균등, `margin-right`에 적용시 element 오른쪽에, `margin-left`에 적용시 element 왼쪽에 margin이 생깁니다. (자동으로)
	- top과 bottom에는 적용이 되지 않습니다.
- 예시

	```html
	<!DOCTYPE html>
	<html>
	<head>
	<style>
		div {
		  width:300px;
		  margin: auto;
		  border: 1px solid red;
		}
	</style>
	</head>
	<body>

		<div>
		This div will be horizontally centered because it has margin: auto;
		</div>

	</body>
	</html>
	```
	![margin-auto](https://i.imgur.com/s4gN1HS.png)

***

## The inherit value

`margin` 속성으로 `inherit`으로 지정함으로써, 해당 element의 부모 element margin 속성값을 inherit 할 수 있습니다.

- 만약 부모 element의 margin 속성값이 지정되어 있지 않다면, margin에 있어서 아무것도 표현 및 적용되지 않습니다.

- 예시
	```html
	<!DOCTYPE html>
	<html>
	<head>
	<style>
	  div {
	    border: 1px solid red;
		margin-left: 100px;
	  }

	  p.ex1 {
	    margin-left: inherit;
	  }
	</style>
	</head>
	<body>

	  <div>
	  <p class="ex1">This paragraph has an inherited left margin (from the div element).</p>
	  </div>

	</body>
	</html>
	```
	![margin-inherit](https://i.imgur.com/X9hl9mx.png)
