# HTML, CSS 

<br/>

## HTML 사용법(문법)

### Contents

- [Anchor](#anchor)
- [Image](#image)
- [목록 List](#list)
- [정의 리스트 Description List](#description)
- [인용 Quotations](#quotations)
- [Form 태그](#form)
- [표 Table](#table)
- [Media](#media)

<br/>

## Anchor
현 위치에서 다른 위치로 이동

## Anchor(Target="_blank")
새 탭 후 해당 위치로 이동
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Anchor</title>
    </head>
    <body>
        <h1>Be Really Excellent</h1>
        <h2>구름EDU 클라우드 SW교육환경</h2>
        <p>
            스크래치3, 엔트리부터 파이썬, C언어까지 설치가 전혀 필요없고
            <br />
            강력한 LMS와 연동된 SW교육환경이 눈앞에 펼쳐집니다.
            <br />
            누구나 SW에 대한 지식과 경험을 나눌 수 있고, 누구나 SW를 배울 수 있는 환경! 지금 경험해보세요!
            <br />
            <br />
        </p>
        <a
            href="https://edu.goorm.io/learn/lecture/20583/%EA%B9%80%EB%B2%84%EA%B7%B8%EC%9D%98-html-css%EB%8A%94-%EC%9E%AC%EB%B0%8C%EB%8B%A4/lesson/976524/%EB%A7%81%ED%81%AC-anchor/image/1"
        >
            서비스 바로가기
        </a>

        <br />
        <br />
        <br />
        <a href="https://github.com/JJongPang?tab=repositories" target="_blank">
            <h1>Subscribe Jonghyeon</h1>
            <p>이 배너를 클릭하시면 이종현의 git 이동합니다.</p>
        </a>
    </body>
</html>
```

<br/>

## Image
이미지 태그

```md
<img src="" alt="" />
```

<br/>

## List
ul과 ol의 자식 요소는 무조간 li만 가능
#### ul
순서가 중요하지 않은 목록
```html
<ul>
	<li>항목</li>
   	<li>항목</li>
</ul>
```
#### ol
순서가 중요한 목록
```html
<ol>
	<li>항목</li>
   	<li>항목</li>
</ol>
```

<br/>

## Description
- 용어를 정의할 때 사용하는 정의리스트
- key-value로 정보를 제공할 때


태그정의
```md
dl(description list), 
dt(description term), 
dd(description data), 
dfn
```

예제
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Description List</title>
</head>
<body>
    
<!-- 예제1 -->
<dl>
    <dt>
        <h1>학습 學習 [학씁]</h1>
    </dt>
    <dd>
        1. noun 배워서 익힘.
    </dd>
    <dd>
        2. noun 심리 경험의 결과로 나타나는, 비교적 지속적인 행동의 변화나 그 잠재력의 변화. 또는 지식을 습득하는 과정
    </dd>
</dl>

<!-- 예제2 -->
<dl>
    <dt>OPEN</dt>
    <dd>월요일</dd>
    <dd>화요일</dd>
    <dd>수요일</dd>
    <dd>목요일</dd>
    <dd>금요일</dd>

    <dt>CLOSE</dt>
    <dd>토요일</dd>
    <dd>일요일</dd>
    <dd>공휴일</dd>
</dl>

<!-- 예제3 -->
<dl>
    <div>
        <dt>USERNAME</dt>
        <dd>김버그</dd>
    </div>
    <div>
        <dt>EMAIL</dt>
        <dd>JONG-HYEOIN@JONGHYEON.com</dd>
    </div>
    <div>
        <dt>PASSPORT#</dt>
        <dd>M@@@@@@@@@@</dd>
    </div>
    <div>
        <dt>NATIONALITY</dt>
        <dd>Republic of Korea</dd>
    </div>
</dl>

</body>
</html>
```

<br/>

## Quotations
```md
<blockquote cite="https://www.naver.com">인용내용</blockquote>
<cite>인용 출처</cite>
<q></q>
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Quotations</title>
    </head>
    <body>
        <blockquote>
            우리가 겪을 수 있는 가장 아름다운 체험은 신비다.<br />
            신비는 모든 참 예술과 과학의 근원이다.<br />
            <cite>- 알버트 아인슈타인</cite>
        </blockquote>

        <blockquote cite=" https://bit.ly/2mvSYrT">
            <p>
                The study is the first to project the long-term outlook for Antarctica's largest penguins, which can grow 1.2 meters (four
                ft) tall, seeking to fill a gap in understanding climate change and wildlife in one of the remotest parts of the planet.
            </p>
            <p>
                Overall, numbers were set to fall by at least 19 percent from current levels by 2100 as sea ice melts. And two-thirds of
                colonies of the birds, which have distinctive golden head patches, would decline by more than half, it said.
            </p>

            <p>
                <q>It's not happy news for the emperor penguin</q>,said Hal Castellan of the U.S. Woods Hole Oceanographic Institution, a
                co-author of the study in the journal Nature Climate Change.
            </p>
            <cite>
                “Emperor Penguin Population to Slide Due to Climate Change”, Scientific American, June 29, 2014, https://bit.ly/2mvSYrT
            </cite>
        </blockquote>
    </body>
</html>
```

<br />

## Form
사용자로부터 Input을 받기 위한 태그

```md
<form action="API주소" method="GET/POST"></form>
```

## Input
입령창, input field
```md
<input type="?" placeholder="이름" minlength="5" maxlength="13" required value="???" />

attribute
1.placeholder = 입력창 문구
2.minlength = 최소 길이
3.maxlength = 최대 길이
4.required = 무조건 입력
5.value = 기본값

type
1.text
2.email
3.password
4.url
5.number(min, max)
6.file(accept=".png, .jpeg")
```


## Label
폼 양식에 이름을 붙이는 태그
```md
<label for="user-name">이름</label>
<input id="user-name" type="text" />
```

## Radio & Checkbox
Radio box 단일 선택
```md
<input id="subscribed" name="subscribed" value="subscribed" type="radio" />
<label for=subscribed">구독중</label>
<input id="unsubscribed" name="subscribed" value="unsubscribed" type="radio" />
<label for=unsubscribed">구독 취소</label>
```

Checkbox 다중 선택
```md
<input type="checkbox" name="skills" value="html" id="html" />
<label for="html">html</label>
<input type="checkbox" name="skills" value="css" id="css" />
<label for="css">css</label>
<input type="checkbox" name="skills" value="js" id="js" />
<label for="js">js</label>
<input type="checkbox" name="skills" value="react" id="react" />
<label for="react">react</label>
```

## Select & Option
```md
<label for="skills">스킬</label>
<select name="skills" id="skills">
	<option value="html">HTML</option>
	<option value="css">CSS</option>
	<option value="javascript">JavaScript</option>
</select>
```

## Textarea
```md
<textarea name="" id="" cols="30" rows="10"></textarea>
```

## Buttons
```md
<button type="submit/button/reset">제출하기</button>
```

<br />

## Table
```md
<table>
	<tr>
 		<th>테이블 헤더</th>
        <td>테이블 데이터</td>
 	</tr>
</table>

*attribute
테이블 헤더 표시 tag
<thead></thead>

테이블 데이터 표시 tag
<tbody></tbody>

테이블에 최종 결과물 tag
<tfoot></tfoot>    
```

<br />

## Media
```md
<audio src="" controls></audio>
<video src="" controls></video>
<!-- iframe -->
<!-- 임베디드 할 때 -->
<iframe src="https://edu.goorm.io" frameborder="0"></iframe>

*attribute
controls = audio 컨트롤러
autoplay = 자동재생
loop autoplay = 무한 반복 재생
```

### 1. 테이블 그리기

- 기본적으로 열을 나누는 방법은 `|`을 사용하는 방법이다.(`\`\_역슬레쉬 위에 있는 문자)

```

|기본적으로|역슬래쉬로|구간나누기|

```

:point_right: **Example**

| 기본적으로 |역슬래쉬로|구간나누기|

- 그러나 그냥 한 줄만 작성할 경우 테이블이 생기지 않는다.

```

|기본적으로|역슬래쉬로|구간나누기|
|-|-|-|

```

:point_right: **Example**

| 기본적으로 | 역슬래쉬로 | 구간나누기 |
|-|-|-|

<br/>

- 위의 내용처럼 하단에 행 수만큼의 `-`를 적어주게 되면 그때부터 테이블이 생성되기 시작한다.
- `-`을 기준으로 위에는 **header가** 되며 아래는 내용들이 된다.

:point_right: **Example**

```

| 기본적으로 | 역슬래쉬로 | 구간나누기 |
|-|-|-|
|왼쪽|가운데|오른쪽|
|왼쪽2|가운데2|오른쪽2|

```

:point_right: **Example**

| 기본적으로 | 역슬래쉬로 | 구간나누기 |
|-|-|-|
|왼쪽|가운데|오른쪽|
|왼쪽2|가운데2|오른쪽2|

<br/>

### 2. 정렬하기

- 테이블에서 잘 쓰이는 것이 정렬이다.
- 정렬의 종류는 3가지로 왼쪽, 가운데, 오른쪽 정렬이 있다.
- 정렬의 구분은 `:`를 사용해서 구분한다.
- 왼쪽 정렬 `:-`, 가운데 정렬 `:-:`, 오른쪽 정렬 `-:`이다.

```md
| 기본적으로 | 역슬래쉬로 | 구간나누기 |
|:-|:-:|-:|
|왼쪽|가운데|오른쪽|
|왼쪽2|가운데2|오른쪽2|
```

:point_right: **Example**

| 기본적으로 | 역슬래쉬로 | 구간나누기 |
| :-------- | :-------: | ---------:|
|왼쪽|가운데|오른쪽|
|왼쪽2|가운데2|오른쪽2|

<br/>

---

## 숨김, 열림

```md
<details>
<summary> 열기 </summary>

- [Memoization](https://github.com/Im-D/Dev-Docs/blob/master/Design_Pattern/Memoization.md)
- [쓰로틀링과 디바운싱](https://github.com/Im-D/Dev-Docs/blob/master/Design_Pattern/Throttle%20and%20Debounce.md)

</details>
```

:point_right: **Example**

<details>
<summary> 열기 </summary>

- [Memoization](https://github.com/Im-D/Dev-Docs/blob/master/Design_Pattern/Memoization.md)
- [쓰로틀링과 디바운싱](https://github.com/Im-D/Dev-Docs/blob/master/Design_Pattern/Throttle%20and%20Debounce.md)

</details>

<br/>

---

## YouTube

```md
  [![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/BVRcKLOEmF8/0.jpg)](http://www.youtube.com/watch?v=BVRcKLOEmF8)
```

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/BVRcKLOEmF8/0.jpg)](http://www.youtube.com/watch?v=BVRcKLOEmF8)

---

####  Reference

- [[공통] 마크다운 markdown 작성법](https://gist.github.com/ihoneymon/652be052a0727ad59601)
- [스티브잡스의 9가지 명언](http://bonlivre.tistory.com/382)
- [MarkDown Cheatsheet](http://assemble.io/docs/Cheatsheet-Markdown.html)