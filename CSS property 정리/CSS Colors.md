Colors
======

<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
<!-- code_chunk_output -->

- [Background Colors](#background-colors)
- [Text Color](#text-color)
- [Border Color](#border-color)

<!-- /code_chunk_output -->

## Background Colors   
- `background-color:색깔`
	- HTML element의 배경색을 설정할 수 있다.   

- 예시

  ```html
  <!DOCTYPE html>
	<html>
	<body>

	  <h1 style="background-color:DodgerBlue;">Hello World</h1>

      <p style="background-color:Tomato;">
	   Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.
	   Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.
	  </p>

	</body>
	</html>
  ```
  ![Color-background](https://i.imgur.com/BMKL6Fi.jpg)

## Text Color
- `color:색깔`
	- 텍스트의 색깔을 설정할 수 있다.
- 예시

  ```html
  <!DOCTYPE html>
  <html>
  <body>

    <h3 style="color:Tomato;">Hello World</h3>

    <p style="color:DodgerBlue;">Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>

    <p style="color:MediumSeaGreen;">Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>

  </body>
  </html>
  ```

  ![Color-text](https://i.imgur.com/Jm8tN1g.jpg)

## Border Color
- `border: 픽셀값 선_종류 색깔`
	- border(가장자리)의 색깔을 설정할 수 있다.
	- 픽셀값과 선_종류가 유효해야, 색깔이 적용된 것을 확인할 수 있다.

- 예시

	```html
	<!DOCTYPE html>
  	<html>
  	<body>

      <h1 style="border: 2px solid Tomato;">Hello World</h1>

      <h2 style="border: 2px solid DodgerBlue;">Hello World</h2>

      <p style="border: 2px solid Violet;">Hello World</p>

  	</body>
  	</html>
	```
  	![Color-border](https://i.imgur.com/oSsWkkI.jpg)
