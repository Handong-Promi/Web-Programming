Paragraphs
==========

1.	`<p>`

	-	**CONCEPT**
		-	`<p>` element는 하나의 paragraph(단락)를 명시합니다.
		-	한 paragraph는 **항상 새로운 줄에서 시작**하며, 브라우저는 자동으로 해당 **paragraph의 전후(위 아래)에 약간의 공백(margin)을 추가**합니다.
	-	**예시**

		```html
		<!DOCTYPE html>
		<html>
		<body>
		  <p>This is a paragraph.</p>
		  <p>This is a paragraph.</p>
		  <p>This is a paragraph.</p>
		</body>
		</html>
		```

		![paragraph-p](https://i.imgur.com/KF9Tcj8.png)

2.	`<hr>`

	-	**CONCEPT**
		-	`<hr>` 태그는 HTML 페이지 안에서 **주제를 구분**할 때 사용되며, 주로 하나의 수평 구분선 (horizontal rule)을 표시합니다.
	-	**예시**

		```html
		<!DOCTYPE html>
		<html>
		<body>
		    <h1>This is heading 1</h1>
		    <p>This is some text.</p>
		    <hr>
		    <h2>This is heading 2</h2>
		    <p>This is some other text.</p>
		    <hr>
		    <h2>This is heading 2</h2>
		    <p>This is some other text.</p>
		</body>
		</html>
		```

		![paragraphs-hr](https://i.imgur.com/yZiQiWD.png)

3.	`<br>`

	-	**CONCEPT**

		-	`<br>` 태그는 개행할 때에 사용합니다.
		-	마지막에 /를 붙인 `<br/>`로도 사용할 수 있습니다.

	-	**예시**

		```html
		<!DOCTYPE html>
		<html>
		<body>
		  <p>This is<br>a paragraph<br>with line breaks.</p>
		</body>
		</html>
		```

		![paragraphs-br](https://i.imgur.com/MS6MLN9.png)

4.	`<pre>`

	-	**CONCEPT**

		-	`<pre>` 태그는 **미리 정의된 형식(preformatted)의 텍스트**를 정의할 때 사용합니다.
		-	`<pre>` 요소 내의 텍스트는 시스템에서 미리 지정된 고정폭 글꼴(fixed-width font)을 사용하여 표현되며, **텍스트에 사용된 여백과 줄바꿈이 모두 그대로 브라우저 화면에 나타납니다.**
		-	이러한 `<pre>` 요소를 사용하면, 독특한 서식의 텍스트나 컴퓨터 코드 등을 HTML 문서에 그대로 표현할 수 있습니다.

			[(출처:TCP school)](http://tcpschool.com/html-tags/pre)

	-	**예시**

		```html
		<!DOCTYPE html>
		<html>
		<body>  
		  <p>The pre tag preserves both spaces and line breaks:</p>
		  <pre>
		    My Bonnie lies over the ocean.


		    My Bonnie lies over the sea.
		    My Bonnie lies over the ocean.
		    Oh, bring back my Bonnie to me.
		  </pre>
		</body>
		</html>
		```

		![Paragraphs-pre](https://i.imgur.com/oUqQ7Q6.png)
