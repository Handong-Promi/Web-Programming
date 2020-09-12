head tag and his children.
==========================

1.	**`<head>`**

	-	**CONCEPT**

		-	`<head>` element는 **meta data**를 포함하는 컨테이너이다.

			-	meta data는 HTML document에 대한 데이터이다.
			-	meta data는 실제 화면 상에 표현되지 않는다.
			-	meta data는 전형적으로 document title, character set, styles, scripts, and other meta information 등을 정의한다.

		-	`<html>` 태그와 `<body>` 태그 사이에 위치한다.

		-	`<head>` element 안에는 아래의 element(태그)들이 들어갈 수 있다.

			-	`<title>`
			-	`<style>`
			-	`<base>`
			-	`<link>`
			-	`<meta>`
			-	`<script>`
			-	`<noscript>`

	-	**예시**

		```html
		<!DOCTYPE html>
		<html lang="en">
		<head>
		  <title>Title of the document</title>
		  <style>
		    body {
		        min-width:900px;
		    }
		  </style>
		</head>
		<body>
		    <h1>This is a heading</h1>
		    <p>This is a paragraph.</p>
		</body>
		</html>
		```

2.	**`<title>`**

	-	**CONCEPT**

		-	`<title>` 태그에서는 해당 문서의 제목을 정의합니다.

			-	제목은 오직 '문자'여야하며, 브라우저의 title bar 혹은 페이지 탭에 표시됩니다.

				![title](https://i.imgur.com/sDmMMkg.png)  
				 > 위 이미지에서 'HTML title tag'에 해당하는 부분이 바로 `<title>` 태그 안에서 정의된, 해당 문서의 제목입니다.

		-	이 태그는 모든 HTML 문서에 꼭 필요합니다.

		-	한 HTML 문서에는 오직 하나의 `<title>` element만이 존재할 수 있습니다.

	-	**예시**

		```html
		<!DOCTYPE html>
		<html lang="en">
		<head>
		  <title>여기가 바로 HTML 문서의 제목을 네이밍할 수 있는 곳!!</title>
		  </style>
		</head>
		```

3.	**`<style>`**

	-	**CONCEPT**
		-	`<style>` 태그는 **해당 문서의 스타일 정보 (CSS)를 정의**할 때 사용합니다.
		-	`<style>` element 안에서, 브라우저 상에서 HTML element들이 어떻게 렌더링되어야 하는지 구체화(정의)할 수 있습니다.
		-	먄약 서로 다른 style sheets에서 동일한 selector에 대해 CSS를 적용했다면, 마지막으로 읽힌(존재하는) style sheet가 사용됩니다.
	-	**예시**

		```html
		<html>
		<head>
		  <style>
		    h1 {color:red;}
		    p {color:blue;}
		  </style>
		</head>
		<body>
		  <h1>Hello world</h1>
		  <p>This is promi!</p>
		```

		-	결과  
			![style](https://i.imgur.com/byg9avZ.png)

4.	**`<base>`**

	-	**CONCEPT**
		-	`<base>` 태그는 문서 안의 모든 상대(relative) URL이 사용할 기준(base) URL을 지정합니다.
		-	`<base>` 태그에는 href 혹은 target 속성이 있거나 둘 다 있어야합니다.
		-	하나의 문서에는 오직 하나의 `<base>` element만이 존재할 수 있으며, `<head>` element 안에 있어야합니다.
	-	**예시**

		```html
		<head>
		  <base href="https://www.w3schools.com/" target="_blank">
		</head>


		<body>
		  <img src="images/stickman.gif" width="24" height="39" alt="Stickman">
		  <a href="tags/tag_base.asp">HTML base Tag</a>
		</body>
		```

		-	설명
			-	상대 URL은 images/stickman.gif와 tags/tag_base.asp입니다.
			-	그 앞에 '기준'이 될 URL은 바로 `<head>` element 안 `<base>` 태그의, https://www.w3schools.com/ 입니다.

5.	**`<link>`**

	-	**CONCEPT**
		-	현재 문서와 외부 리소스 간의 관계를 정의합니다.  
		-	주로 외부 style sheets를 연결하는 용도로 사용됩니다.
	-	**예시**

		```html
		<!DOCTYPE html>
		<html>
		<head>
		  <link rel="stylesheet" href="styles.css">
		</head>
		<body>
		  <h1>Hello World!</h1>
		  <h2>I am formatted with a linked style sheet.</h2>
		  <p>Me too!</p>
		</body>
		</html>
		```

		-	설명
			-	`href`: 외부 리소스의 경로
			-	`rel`: 현재 문서와 연결한 아이템의 **관계**가 어떻게 되는지 설명

6.	**`<meta>`**

	-	**CONCEPT**

		-	meta태그는 **meta data(정보에 대한 정보)를 제공**하는 역할을 합니다.
		-	character set, page description, keywords, author, view point setting 등을 정의할 수 있습니다.
		-	화면에는 별달리 표시되는 것이 없지만, **검색 엔진이나 브라우저에 읽힙니다.** [(출처: [html] meta 태그 사용법 :: 지구별 안내서)](https://aboooks.tistory.com/339)

	-	**예시**

		1.	검색 엔진을 위한 키워드

			```html
			<meta name="keywords" content="HTML, markdown, promi, HGU">
			```

		2.	웹 페이지 설명

			```html
			<meta name="description" content="html 기본 태그 정리">
			```

		3.	웹 페이지 저자(author)

			```html
			<meta name="author" content="Promi">
			```

		4.	view point

			```html
			<meta name="viewport" content="width=device-width, initial-scale=1.0">
			```

7.	**`<script>`**

	-	To be described

8.	**`<noscript>`**

	-	To be described
