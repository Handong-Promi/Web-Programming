Block & Inline Elements
=======================

---

> 시작 전, 이 문서는 w3schools의 [HTML Block & Inline Elements](https://www.w3schools.com/html/html_blocks.asp)을 참고하였음을 밝힙니다.

---

모든 HTML element는, 자신의 타입에 따른 default display 값이 있습니다.  
display 값에는 두 가지가 있습니다; **Block** & **Inline**

Block-level Elements
--------------------

Block-level element는 항상 새로운 줄에서 시작하며, 가능한 한 최대의 width를 차지합니다(최대한 가능한 만큼의 좌우로 쭉 뻗습니다).

Ex) `<div>`, `<article>`, `<pre>`, `<footer>` 등

Inline Elements
---------------

Inline element는 새로운 줄에서 시작되지 않으며, 필요한 width만큼만을 차지합니다.

Ex) `<a>`, `<button>`, `<span>` 등  
> Inline element는 Block-level element를 포함할 수 없습니다.

---

Block-level Element와 Inline element의 대표; \<div> & \<span>
-------------------------------------------------------------

1.	`<div>`

	-	**CONCEPT**

		-	`<div>` element는 다른 HTML element들을 위한 'container'로 자주 사용됩니다.
		-	`<div>` element에 필수(요구로 되는) 속성은 없지만, `style`, `class`, `id`가 흔히 사용됩니다.
		-	CSS와 함께 사용할 경우, `<div>` element를 사용하여 컨텐츠 block을 스타일링할 수 있습니다.

		Good to refer: [[Html] Div 태그 사용법 & 예제](https://coding-factory.tistory.com/188)

	-	**예시**

		```html
		<!DOCTYPE html>
		<html>
		<body>
		  <div style="background-color:black;color:white;padding:20px;">
		    <h2>London</h2>
		    <p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
		    <p>Standing on the River Thames, London has been a major settlement for two millennia, its history going back to its founding by the Romans, who named it Londinium.</p>
		 </div>
		</body>
		</html>
		```

		![block&Inline-div](https://i.imgur.com/cyb7nyh.png)

2.	`<span>`

	-	**CONCEPT**
		-	`<span>` element는 텍스트의 일부 혹은 문서의 일부를 표시(mark up)하기 위해 사용되는 inline container입니다.
		-	`<span>` element에 필수(요구로 되는) 속성은 없지만, `style`, `class`, `id`가 흔히 사용됩니다.
		-	CSS와 함께 사용할 경우, `<span>` element를 사용하여 텍스트의 일부를 스타일링할 수 있습니다.
	-	**예시**

		```html
		<!DOCTYPE html>
		<html>
		<body>
		  <h1>The span element</h1>
		  <p>My mother has <span style="color:blue;font-weight:bold">blue</span> eyes and my father has <span style="color:darkolivegreen;font-weight:bold">dark green</span> eyes.</p>
		</body>
		</html>
		```

		![block&Inline-span](https://i.imgur.com/RfpXdgW.png)
