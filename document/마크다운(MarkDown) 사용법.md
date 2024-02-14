# [마크다운(MarkDown)](https://daringfireball.net/projects/markdown)

## Markdown이란 

마크다운 (Markdown)은 마크업 언어의 일종으로, 존 그루버(John Gruber)와 아론 스워츠(Aaron Swartz)가 만들었습니다. <br>
마크다운은 텍스트 기반의 마크업 언어로, 문서를 쉽게 작성하고 편집할 수 있도록 도와주는 간단한 형식 지정 언어입니다. <br>

#### 존 그루버의 블로그를 통한 마크다운의 장점으로는
1. 간편함: Markdown은 간단하고 직관적인 문법을 사용하기 때문에 사용자가 빠르게 익힐 수 있습니다. 복잡한 마크업 언어보다 훨씬 쉽게 문서를 작성할 수 있습니다.
2. 가독성: Markdown으로 작성된 문서는 일반 텍스트로도 읽을 수 있기 때문에 가독성이 뛰어납니다. 또한 Markdown 문법은 텍스트의 구조를 명확하게 표현하여 문서의 구조를 쉽게 파악할 수 있도록 도와줍니다.
3. 지원되는 플랫폼: Markdown은 다양한 플랫폼에서 지원되며, 대부분의 텍스트 편집기나 온라인 플랫폼에서 사용할 수 있습니다. 이는 Markdown으로 작성된 문서를 다양한 환경에서 쉽게 공유하고 편집할 수 있음을 의미합니다.
4. 웹 호환성: Markdown 문서는 HTML로 변환이 가능하며, 웹 페이지에 쉽게 삽입할 수 있습니다. 따라서 Markdown을 사용하면 웹에서도 문서를 보기 쉽게 표현할 수 있습니다.
5. 확장성: Markdown은 확장 가능한 언어이기 때문에 필요에 따라 사용자 정의 기능을 추가하여 더 다양한 형식의 문서를 작성할 수 있습니다. 이를 통해 Markdown을 다양한 용도로 활용할 수 있습니다.

# Markdown Elements
## contents
[1. Headers 헤더](#1-headers-헤더)<br>
[2. Emphasis 강조](#2-emphasis-강조)<br>
[3. Blockquotes 인용](#3-blockquotes-인용)<br>
[4. Lists 목록](#4-lists-목록)<br>
[5. Backslash Escapes 백슬래쉬 이스케이프](#5-backslash-escapes-백슬래쉬-이스케이프)<br>
[6. Images 이미지](#6-images-이미지)<br>
[7. Links (Anchor) 링크](#7-links-anchor-링크)<br>
[8. Fenced Code Blocks 코드 블럭](#8-fenced-code-blocks-코드-블럭-(빽틱))<br>
[9. Task Lisk 체크 리스트](#9-task-lisk-체크-리스트)<br>
[10. Horizontal Rules 수평선](#10-horizontal-rules-수평선)<br>
[11. Emoji 이모티콘](#11-emoji-이모티콘)<br>
[12. Table 테이블](#12-table-테이블)<br>
[13. Line Breaks 줄바꿈](#13-line-breaks-줄바꿈)<br>
[14. Comments 참고 링크](#14-Comments-참고-링크)<br>
[16. Reference 참고 링크](#15-reference-참고-링크)<br>

## 1. Headers 헤더
* `#`으로 시작하는 텍스트.
* `#`은 하나부터 여섯개까지 가능.
* `#`이 늘어날때마다 제목의 스케일 작아집니다.
* H1은 `===`로도 만들 수 있습니다.
* H2는 `---`로도 만들 수 있습니다.
  
### Syntax 마크다운 사용법
    This is an H1
    ===
    This is an H2
    ---
    # This is an H1
    ## This is an H2
    ### This is an H3
    #### This is an H4
    ##### This is an H5
    ###### This is an H6    
### Headers 실행결과
H1<br>
===
H2<br>
---
# H1; <br>
## H2; <br>
### H3; <br>
#### H4; <br>
##### H5; <br>
###### H6; <br>

## 2. Emphasis 강조
* 기울여 쓰기(italic) : `*` 또는 `_`로 감싼 텍스트.
* 두껍게 쓰기(bold) : `**` 또는 `__`로 감싼 텍스트.
* 취소선 : `~~`로 감싼 텍스트.
* 이태릭체와 볼드를 같이 사용할 수 있습니다.
  
### Syntax 마크다운 사용법
      *기울여 쓰기*
      _기울여 쓰기_
      **두껍게 쓰기**
      __두껍게 쓰기__
      ~~취소선입니다.~~
      *기울게 **두껍게** 동시사용 가능*      
### Emphasis 실행결과
*기울여 쓰기 실행결과* <br>
_기울여 쓰기 실행결과_ <br>
**두껍게 쓰기 실행결과** <br>
__두껍게 쓰기 실행결과__ <br>
~~취소선입니다.~~ <br>
*기울여 **두껍게** 동시 사용가능* <br>

## 3. Blockquotes 인용
* `>`으로 시작하는 텍스트.
* `>`는 3개까지 가능합니다.
* `1개`는 인용문.
* `2개`는 인용문 안에 인용문.
* `3개`는 인용문 안에 인용문 안에 인용문.
  
### Syntax 마크다운 사용법
    인용문:
    > 인용문1.
    > > 인용문2.
    > > > 인용문3.
### Demonstration 실행결과
인용문:
> 인용문1.
> > 인용문2.
> > > 인용문3.

## 4. Lists 목록
### 4.1. Unordered lists 순서가 없는 목록
* `*`, `+`, `-` 를 이용해서 순서가 없는 목록을 만들 수 있습니다.
* 들여쓰기를 하면 모양이 바뀝니다.
### 4.2. Ordered lists 순서가 있는 목록
* 숫자를 기입하면 순서가 있는 목록이 됩니다.
* 들여쓰기를 하면 모양이 바뀝니다.
### Syntax 마크다운 사용법
    * Item 1
    * Item 2
      * Item 1
        * Item 1

### Lists 실행결과
* Item 1
* Item 2
  * Item 1
    * Item 1
    
## 5. Backslash Escapes 백슬래쉬 이스케이프
* 특수문자를 표현할 때, 표시될 문자 앞에 `\`를 넣고 특수문자를 쓰면 됩니다.
* 주의할 점은 앞과 뒤에가 형식이 똑같이 백슬래쉬 뒤에 특수문자입니다. `감싸는 형태가 아닙니다.`
* 백슬래쉬는 아래의 특수문자를 표현할 수 있습니다.
* \ backslash, \ backtick, * asterisk, _ underscore, {} curly braces, [] square brackets,
() parentheses, # hash mark, + plus sign, - minus sign (hyphen), . dot, ! exclamation mark
### Syntax 마크다운 사용법
	\*literal asterisks\*
	\#hash mark\#
	\[squre brackets\]
### Lists 실행결과
\*literal asterisks\* <br>
\#hash mark\# <br>
\[squre brackets\] <br>

## 6. Images 이미지
* <img>로 변환됩니다.
* 링크와 비슷하지만 앞에 `!`가 붙습니다.
* 인라인 이미지 \![alt text](/test.png\)
* 링크 이미지 \![alt text](image_URL\)
* 이미지의 사이즈를 변경하기 위해서는 `<img width="OOOpx" height="OOOpx"></img>`와 같이 표현합니다.
### Syntax 마크다운 사용법
	![alt 잘생긴 내얼굴](/img/tomato.jpg)
  
### Images 실행결과
<br>
<br>
<br>

## 7. Links (Anchor) 링크
## 7.1. External Links 외부 링크
	인라인 링크: [링크](http://example.com "링크 제목")
	url 링크: <example.com>, <example@example.com>; 꺽쇠 괄호 없어도 자동으로 링크를 사용
### Syntax 마크다운 사용법
	[Google](http://www.google.com "구글")
	www.google.com
### External Links 실행결과
[Google](http://www.google.com "구글") <br>
www.google.com

## 7.2. Internal Links 내부 링크
	[보여지는 내용](#이동할 헤드(제목))
	괄호 안의 링크를 쓸 때는 띄어쓰기는 -로 연결, 영어는 모두 소문자로 작성
### Syntax 마크다운 사용법
	[1. Headers 헤더](#1-headers-헤더)
	[2. Emphasis 강조](#2-emphasis-강조)
	[3. Blockquotes 인용](#3-blockquotes-인용)
### Links 실행결과
[1. Headers 헤더](#1-headers-헤더)<br>
[2. Emphasis 강조](#2-emphasis-강조)<br>
[3. Blockquotes 인용](#3-blockquotes-인용)<br>

## 8. Fenced Code Blocks 코드 블럭 (빽틱)
* 간단한 인라인 코드는 텍스트를 앞뒤로 \`기호로 감싸면 됩니다.
* \`\`\` 혹은 ~~~ 코드.
* 첫 줄과 마지막 줄에 Back quote ( \` ) 또는 물결( ~ ) 3개 삽입.
* 코드가 여러 줄인 경우, 줄 앞에 공백 네 칸을 추가하면 됩니다.
* \`\`\` 옆에 언어를 지정해주면 syntax color가 적용됩니다.
### Syntax 마크다운 사용법
	```
	코드를 작성할 수 있습니다.
	```
	~~~
	코드를 작성할 수 있습니다.
	~~~
		4 spaces
	```javascript
	function test() {
	 console.log("코드를 작성할 수 있습니다.");
	}
	```
### Fenced Code Blocks 실행결과
```
코드를 작성할 수 있습니다.
```
~~~
코드를 작성할 수 있습니다.
~~~
	4 spaces
```javascript
function test() {
 console.log("코드를 작성할 수 있습니다.");
}
```

## 9. Task Lisk 체크 리스트
* 줄 앞에 `- [x]`를 써서 완료된 리스트 표시.
* 줄 앞에 `- [ ]`를 써서 미완료된 리스트 표시.
* 체크 안에서 강조 외에 여러 기능을 사용할 수 있습니다.
### Syntax 마크다운 사용법
    - [x] checked === true     
    - [ ] checked === false
### Task Lisk 실행결과
- [x] checked === true
- [ ] checked === false

## 10. Horizontal Rules 수평선
* \- 또는 * 또는 _ 을 3개 이상 작성.
* 단, -을 사용할 경우 header로 인식할 수 있으니 이 전 라인은 비워두어야 합니다.
### Syntax 마크다운 사용법
	* * *
	***
	*****
	- - -
	-------------------
### Horizontal Rules 실행결과
* * *
***
*****
- - -
-------------------

## 11. Emoji 이모티콘
* 마크다운을 이용해 이모티콘을 표현가능.
* github에서 마우스 우 클릭 후 그림 이모티콘 클릭 후 사용가능.

### Syntax 마크다운 사용법
	:thumbsup
### Emoji 실행결과
👍

## 12. Table 테이블
* 헤더와 셀을 구분할 때 3개 이상의 `-`(hyphen/dash) 기호가 필요합니다.
* 헤더 셀을 구분하면서 :(Colons) 기호로 셀(열/칸) 안에 내용을 정렬할 수 있습니다.
* 가장 좌측과 가장 우측에 있는 |(vertical bar) 기호는 생략 가능합니다.
### Syntax 마크다운 사용법
	테이블 생성

	header1|header2|header3|header4
	---|---|---|---
	cell1|cell2|cell3|cell4
	cell5|cell6|cell7|cell8
	cell9|cell10|cell11|cell12

	테이블 정렬

	header1|header2|header3|header4
	:---|:---:|---:|:---:
	Left|Center|Right|Center
	cell1|cell2|cell3|cell4
	cell5|cell6|cell7|cell8
	cell9|cell10|cell11|cell12
 
### Table 실행결과
테이블 생성

header1|header2|header3|header4
---|---|---|---
cell1|cell2|cell3|cell4
cell5|cell6|cell7|cell8
cell9|cell10|cell11|cell12

테이블 정렬

header1|header2|header3|header4
:---|:---:|---:|:---:
Left|Center|Right|Center
cell1|cell2|cell3|cell4
cell5|cell6|cell7|cell8
cell9|cell10|cell11|cell12

## 13. Line Breaks 줄바꿈
* `<br>`를 활용해서 줄바꿈을 할 수 있습니다. 또는 문장 마지막에서 띄어쓰기를 2번 입력합니다.
### Syntax 마크다운 사용법
	글을 작성하다 줄을 바꾸고 싶어요.
	여기까지는 작성하고 줄 바꿈을 하고 싶습니다. <br>
	쭉 작성하다.
	한번 더 바꾸고 싶어요.<br>
### Line Breaks 실행결과
글을 작성하다 줄을 바꾸고 싶어요.
	여기까지는 작성하고 줄 바꿈을 하고 싶습니다. <br>
	쭉 작성하다.
	한번 더 바꾸고 싶어요.<br>

## 14. comments 주석.
* <!-- -->, [//]: # 기호를 사용해, 주석(Comment)을 표현합니다.
### Syntax 마크다운 사용법
    -- 주 --
    <!-- 주석. -->
    [//]: # (주석.)
    [//]: # "주석."
    [//]: # '주석.'
    -- 석 --
### Comments 실행결과
-- 주 --

<!-- 주석. -->
[//]: # (주석.)
[//]: # "주석."
[//]: # '주석.'

-- 석 --

## 15. Reference 참고 링크
* [Matering Markdown](https://guides.github.com/features/mastering-markdown/)
* [마크다운 위키백과](https://ko.wikipedia.org/wiki/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4)
* [존 그루버의 웹사이트](https://daringfireball.net/projects/markdown/)

