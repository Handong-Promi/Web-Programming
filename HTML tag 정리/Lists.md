Lists
=====

---

> 시작 전, 이 문서는 w3schools의 [HTML Lists](https://www.w3schools.com/html/html_lists.asp)를 참고하였음을 밝힙니다.

---

Unordered HTML List
-------------------

-	**CONCEPT**

	-	순서가 없는 목록은 `<ul>` 태그로 시작합니다.
	-	목록의 각 항목은`<li>`태그로 시작합니다.  
	-	목록의 항목에는 기본적으로 글머리 기호(작은 검은색 원)가 표시됩니다.

-	**예시**

	```html
	<!DOCTYPE html>
	<html>
	<body>
	  <h2>An unordered HTML list</h2>
	    <ul>
	      <li>Coffee</li>
	      <li>Tea</li>
	      <li>Milk</li>
	    </ul>  
	</body>
	</html>
	```

	![lists-unordered](https://i.imgur.com/B1DYNlP.png)

Ordered HTML List
-----------------

-	**CONCEPT**

	-	순서가 있는 목록은 `<ol>` 태그로 시작합니다.
	-	목록의 각 항목은`<li>`태그로 시작합니다.  
	-	목록의 항목에는 기본적으로 각 항목 순서에 맞는 숫자가 표시됩니다.

-	**예시**

	```html
	<!DOCTYPE html>
	<html>
	<body>
	  <h2>An ordered HTML list</h2>
	    <ol>
	      <li>Coffee</li>
	      <li>Tea</li>
	      <li>Milk</li>
	    </ol>  
	</body>
	</html>
	```

	![lists-ordered](https://i.imgur.com/OFOOjSx.png)

HTML Description Lists
----------------------

-	**CONCEPT**
	-	Description 목록은 각 용어에 대한 Description이 포함된, 용어 목록입니다.
	-	`<dl>` 태그는 description list라는 것을 명시하고, `<dt>` 태그는 용어의 이름을 명시하며, `<dd>` 태그에는 각 용어의 대한 description이 들어갑니다.
-	**예시**

	```html
	<!DOCTYPE html>
	<html>
	<body>
	  <h2>A Description List</h2>
	  <dl>
	    <dt>Coffee</dt>
	      <dd>- black hot drink</dd>
	    <dt>Milk</dt>
	      <dd>- white cold drink</dd>
	</dl>
	</body>
	</html>
	```

	![lists-description](https://i.imgur.com/7Pgki1T.png)
