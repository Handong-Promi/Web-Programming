Padding
=======

<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
<!-- code_chunk_output -->

- [Padding](#padding)
- [Individual Sides](#individual-sides)
- [Margin - Shorthand Property](#margin-shorthand-property)

<!-- /code_chunk_output -->

---

> 시작 전, 이 문서는 w3schools의 [CSS Padding](https://www.w3schools.com/css/css_padding.asp)을 참고하였음을 밝힙니다.

---

## Padding

CSS의 `padding` 속성을 이용하여, element의 내용 주변 및 명시 border들의 안쪽 공간을 만들어낼 수 있습니다.

- **Element contents ~ border 경계 사이의 공간을 다루는** CSS 속성이라고 생각하면 됩니다.
- top / right / bottom / left에 있어서 각각의 세팅이 가능합니다.

***

## Individual Sides
1. CSS에서는 한 element의 각 측면에 대한 padding 조정이 가능합니다.

- `padding-top`
- `padding-right`
- `padding-bottom`
- `padding-left`

2. 모든 padding 속성에는 다음과 같은 값들이 올 수 있습니다.
- **length**: px, pt, cm 등의 단위로 padding을 직접 지정합니다.
- **%**: 포함하고 있는 element의 width를 기준으로, 몇 퍼센트를 padding으로 삼을 것인지 지정할 수 있습니다. (너비 백분율 이용)
- **inherit**: 부모 element로부터 padding 값을 받도록 지정할 수 있습니다.

3. length와 %에 있어서, **Negative 값은 불가능**합니다.

4. 예시
	```html
	<!DOCTYPE html>
	<html>
	<head>
	<style>
	  div {
	    border: 1px solid black;
	    background-color: lightblue;
	    padding-top: 50px;
	    padding-right: 30px;
	    padding-bottom: 50px;
	    padding-left: 80px;
	  }
	</style>
	</head>
	<body>

	  <div>이 div element는 top padding을 50px로, right padding을 30px로, bottom padding을 50px로, left padding을 80px로 갖습니다.</div>

	</body>
	</html>
	```
	![padding](https://i.imgur.com/ooBhFJp.jpg)
	![padding-develop](https://i.imgur.com/16Y6xBG.jpg)

***

## Margin - Shorthand Property

`padding` 속성을 통해 `padding-top`, `padding-right`, `padding-bottom`, `padding-left` 네 개의 속성을 한 번에 표현할 수 있습니다.
- `padding`의 속성값이 몇 개인지에 따라, 상하좌우 각각에 어떻게 적용되는지 달라집니다.
	- 1개 : Every side
	- 2개: top & bottm / right & left
	- 3개 : top / right & left / bottom
	- 4새 : top / right / bottom / left

***
