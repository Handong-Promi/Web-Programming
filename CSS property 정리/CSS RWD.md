# CSS Responsive Web Design
***
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
<!-- code_chunk_output -->

- [CSS Responsive Web Design](#css-responsive-web-design)
  - [Introduction](#introduction)
  - [Viewport](#viewport)
    - [What is The Viewport?](#what-is-the-viewport)
    - [Setting The Viewport](#setting-the-viewport)
    - [Size Content to The Viewport; Tip](#size-content-to-the-viewport-tip)
  - [Grid-View](#grid-view)
    - [What is a Grid-View?](#what-is-a-grid-view)
    - [Building a Responsive Grid-View](#building-a-responsive-grid-view)
  - [Media Queries](#media-queries)
    - [What is a Media Query?](#what-is-a-media-query)
    - [Breakpoint](#breakpoint)
      - [1. Add a Breakpoint](#1-add-a-breakpoint)
      - [2. Always Design for Mobile First](#2-always-design-for-mobile-first)
      - [3. Another Breakpoint](#3-another-breakpoint)
      - [4. Typical Device Breakpoints](#4-typical-device-breakpoints)

<!-- /code_chunk_output -->

***

## Introduction
- Responsive web design makes your web page look good on all devices.
- Responsive web design uses **only HTML and CSS.**
- Responsive web design is **not a program or a JavaScript.**

## Viewport

### What is The Viewport?
- The viewport is **the user's visible area of a web page.**
- The viewport varies with the device, and will be smaller on a mobile phone than on a computer screen.

### Setting The Viewport
- `<meta>` tag 이용
	- ```html
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
		```
	- The `width=device-width` part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).
	- The `initial-scale=1.0` part sets the initial zoom level when the page is first loaded by the browser.

### Size Content to The Viewport; Tip
1. **Do NOT use large fixed width elements**
2. **Do NOT let the content rely on a particular viewport width to render well**
3. **Use CSS media queries to apply different styling for small and large screens**
> absolute한 것들보다는 **relative한 것들을 이용하자!**


***

## Grid-View

### What is a Grid-View?
- Many web pages are based on a grid-view, which means that **the page is divided into columns.**
- Using a grid-view is very helpful when designing web pages. **It makes it easier to place elements on the page.**
- A responsive grid-view **often has 12 columns, and has a total width of 100%**, and will shrink and expand as you resize the browser window.

### Building a Responsive Grid-View

- **Step1.**
	모든 HTML elements의 `box-sizing` property를 `border-box`로 설정한다. (border과 padding으로 인해 부여된 width를 벗어나는 경우 방지)
	```CSS
	* {
		box-sizing: border-box;
	}
	```   

- **Step2.**
	1. width를 몇 개의 columns로 나눌 것인지 정한다. (이하 n개)
	2. 한 column당 부여되는 width 공간을 계산한다. (relative하게)
 		- 100% / n

- **Step3.**
	1. `class="col-k"`클래스들 생성....  (1<=k<=n)
	2. **모든 columns들은 floating to left & padding 15px로 설정한다.**

- **Step4.**
	한 row에 같이 쓰고자하는 columns들은 하나의 div로 묶어줘야한다. 즉, 해당 div가 한 row가 되는 것이다.

- **Stpe4.**
	해당 row가 끝나면, floating to left를 해제시켜주어야하므로, 다음과 같은 css style을 삽입해놓는다. (미리)
	```CSS
	.row::after {
  	content: "";
  	clear: both;
  	display: table;
	}
	```

****

## Media Queries

### What is a Media Query?
- Media query is a CSS technique introduced in CSS3.
- It uses the `@media` rule to **include a block of CSS properties only if a certain condition is true.**

### Breakpoint

#### 1. Add a Breakpoint
- 화면의 width 혹은 height에 따라 element를 변경시킬 '기준', 즉 breakpoint를 지정할 수 있다.
- 주로 `max-width` 혹은 `min-width`를 이용한다.
	- `max-width`: 바로 전 breakpoint(없으면 0) ~ 'max-width'까지 media query를 적용
	- `min-width`: 'min-width' ~ 바로 다음 breakpoint(없으면 제한 x)까지 media query를 적용

#### 2. Always Design for Mobile First
- 모바일을 기준으로 해서 breakpoint Design을 하자!

#### 3. Another Breakpoint
- 여러 개의 breakpoint를 명시하여, 보다 세부적으로 media query 적용 구간을 나눌 수 있다.

#### 4. Typical Device Breakpoints
```CSS
/* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {...}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {...}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {...}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {...}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {...}
```
