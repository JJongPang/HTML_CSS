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

## CSS 사용법(문법)

### Contents

- [Box Model](#boxmodel)
- [Float](#float)
- [Position](#position)
- [FlexBox](#flexbox)
- [Typography](#typography)
- [Background](#background)
- [Transition](#transition)
- [Animations](#animations)
- [Selectors](#selectors)
  

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

<br />
<br />

## BoxModel
![](https://images.velog.io/images/whdvkf92/post/467a353f-8a47-45d2-b208-e221729bac7d/BoxModel.JPG)

- Content: 가로 width 세로 height

- Padding: 안쪽 여백, 즉 content와 border 사이의 공간을 나타내는 padding

- Border: 테두리를 타나태는 border

- Margin: 바깥 여백, 즉 요소와 요소 사이의 간격을 나타내는 margin

### Box Sizing
```
box-sizing: border-box/content-box(default)
```

### Box
Block
- 따로 width를 선언하지 않은 경우, width=부모의 content-box의 100%
- 따로 width를 선언한 경우, 남은 공간은 margin으로 자동으로 채움
- margin: 0 auto;
- 따로 부모의 height를 선언하지 않을 경우, 자식 요소의 height의 합=부모의height

Inline
- width, height, padding-top, padding-bottom, border-top, border-bottom, margin-top, - margin-bottom 사용 불가

InlineBlock
- Block, Inline 속성을 가지고 있습니다.

<br />
<br />

## Float
### What Happen
- Block속성 가로배치
- Box의 정의 중 따로 부모의 height를 선언하지 않을 경우, 자식 요소의 height의 합=부모의 height(x)(집 나간 내 새끼, 찾을 길 없네)
- 블록으로 신분 상승
- 길막을 못해 슬픈 블록
- 플로트는 나만 볼 수 있어요(feat. 인라인)

### How to fix
- overflow: hidden; 사용
- clearfix 사용(left, right, both)
- 가상 요소 만들기(Pseudo Element)

<br/>

## Position
### Type => 기준점
- static: 일단 모든 태그들은 처음에 position: static 상태입니다. (기본적으로 static이라 따로 써주지 않아도 됩니다.) 차례대로 왼쪽에서 오른쪽, 위에서 아래로 쌓입니다.
- relative: 여기서 태그의 위치를 살짝 변경하고 싶을 때 position: relative를 사용합니다. 이제 top(위), right(오른쪽), bottom(아래), left(왼쪽) 속성을 사용해 위치 조절이 가능합니다. CSS 탭을 눌러 CSS를 확인해보세요. 각각의 태그가 기존 static이었을 때의 위치를 기준으로 top, right, bottom, left 방향으로 주어진 픽셀만큼 이동했습니다.
- absolute: relative가 static인 상태를 기준으로 주어진 픽셀만큼 움직였다면, absolute는 position: static 속성을 가지고 있지 않은 부모를 기준으로 움직입니다. 만약 부모 중에 포지션이 relative, absolute, fixed인 태그가 없다면 가장 위의 태그(body)가 기준이 됩니다.
- fixed: 제 홈페이지를 보시면 상단 로그인 메뉴와 좌측 내비게이션 메뉴, 우측 명예의 전당, 그리고 하단 포스트 메뉴는 항상 특정 위치에 고정되어 있습니다. 스크롤을 내려도 그 자리에 계속 있죠. 바로 포지션이 fixed로 설정되어 있기 때문입니다. 기준점-viewport
- sticky(x)

<br/>

## FlexBox
## Flexbox
Flex는 요소의 크기가 불분명하거나 동적인 경우에도, 각 요소를 정렬할 수 있는 효율적인 방법을 제공합니다.

우선 Flex는 2개의 개념으로 나뉩니다.
첫 번째는 Container 두 번째는 Items 입니다.
위에서 살펴본 바와 같이 Container는 Items를 감싸는 부모 요소이며, 각 Item을 정렬하기 위해선 Container가 필수입니다.

주의할 부분은 Container와 Items에 적용하는 속성이 구분되어 있다는 것입니다.
Container에는 display, flex-flow, justify-content 등의 속성을 사용할 수 있으며,
Items에는 order, flex, align-self 등의 속성을 사용할 수 있습니다.

![](https://images.velog.io/images/whdvkf92/post/6d36a297-168c-4cea-95db-08c32bc47a41/flex.JPG)


## Flex Container
Flex Container를 위한 속성들은 다음과 같습니다.
주 축(main-axis)과 교차 축(cross-axis)의 개념은 뒤에서 살펴봅시다.

- display: Flex Container를 정의
- flex-flow: flex-direction와 flex-wrap의 단축 속성
- flex-direction: Flex Items의 주 축(main-axis)을 설정
- flex-wrap: Flex Items의 여러 줄 묶음(줄 바꿈) 설정
- justify-content: 주 축(main-axis)의 정렬 방법을 설정
- align-content: 교차 축(cross-axis)의 정렬 방법을 설정(2줄 이상)
- align-items: 교차 축(cross-axis)에서 Items의 정렬 방법을 설정(1줄)

### display
display 속성으로 Flex Container를 정의합니다.
보통 요소의 표시 방법을 display: block;, display: inline-block 혹은 display: none; 같이 사용하는 경우가 많죠.
같은 요소의 표시 방법으로 Block이나 Inline이 아닌 Flex(display: flex, display: inline-flex)로 정의합니다.

- flex: Block 특성의 Flex Container를 정의	
- inline-flex: Inline 특성의 Flex Container를 정의

flex와 inline-flex는 차이는 단순합니다.
display: flex;로 지정된 Flex Container는 Block 요소와 같은 성향(수직 쌓임)을 가지며,
display: inline-flex로 지정된 Flex Container는 Inline(Inline Block) 요소와 같은 성향(수평 쌓임)을 가집니다.

여기서 말하는 수직과 수평 쌓임은 Items가 아니라 Container라는 것에 주의합시다.
두 값의 차이는 내부에 Items에는 영향을 주지 않습니다.![](https://images.velog.io/images/whdvkf92/post/df5a9f60-2df1-465b-a69a-024e1ef963ba/flex-1.JPG)


### flex-flow
이 속성은 단축 속성으로 Flex Items의 주 축(main-axis)을 설정하고 Items의 여러 줄 묶음(줄 바꿈)도 설정합니다.

```css
flex-flow: 주축 여러줄묶음;

.flex-container {
  flex-flow: row-reverse wrap;
}
```
- flex-direction: Items의 주 축(main-axis)을 설정
	row : Itmes를 수평축(왼쪽에서 오른쪽으로)으로 표시
	row-reverse : Items를 row의 반대 축으로 표시
	column : Items를 수직축(위에서 아래로)으로 표시
	Items를 column의 반대 축으로 표시
```css
flex-direction: 주축;
```
![](https://images.velog.io/images/whdvkf92/post/069069d7-099f-4fd1-a040-a6d6575952f5/flex-2.JPG)

주 축(main-axis)과 교차 축(cross-axis)
위에서 언급했었던 주 축(main-axis)과 교차 축(cross-axis)의 개념은 다음과 같습니다.
값 row는 Items를 수평축으로 표시하므로 이때는 주 축이 수평이며 교차 축은 수직이 됩니다.
반대로 값 column은 Items를 수직축으로 표시하므로 주 축은 수직이며 교차 축은 수평이 됩니다.
즉, 방향(수평, 수직)에 따라 주 축과 교차 축이 달라집니다.

![](https://images.velog.io/images/whdvkf92/post/9155d31b-2fcf-4231-9c42-797e74da1336/flex-3.JPG)

시작점(flex-start)과 끝점(flex-end)
시작점(flex-start)과 끝점(flex-end)이라는 개념도 있습니다.
이는 주 축이나 교차 축의 시작하는 지점과 끝나는 지점을 지칭합니다.
역시 방향에 따라 시작점과 끝점이 달라집니다.
![](https://images.velog.io/images/whdvkf92/post/0b35558b-0e4e-4342-9867-dedfb12297ef/flex-4.JPG)
![](https://images.velog.io/images/whdvkf92/post/b4d4dc9a-50de-4df7-bdb3-c788059bc94c/flex-5.JPG)
뒤에서 언급할 속성 중 값으로 flex-start와 flex-end를 사용하는데 이는 방향에 맞는 그 시작점과 끝점을 의미합니다.

- flex-wrap: Items의 여러 줄 묶음(줄 바꿈) 설정	
	nowrap: 모든 Itmes를 여러 줄로 묶지 않음(한 줄에 표시)	nowrap
	wrap: Items를 여러 줄로 묶음	
	wrap-reverse: Items를 wrap의 역 방향으로 여러 줄로 묶음	
```css
flex-wrap: 여러줄묶음;
```
![](https://images.velog.io/images/whdvkf92/post/93776d07-bf45-41ee-9700-9c5666a66638/flex-6.JPG)

### justify-content
주 축(main-axis)의 정렬 방법을 설정합니다.
- flex-start: Items를 시작점(flex-start)으로 정렬	flex-start
- flex-end: Items를 끝점(flex-end)으로 정렬	
- center: Items를 가운데 정렬	
- space-between: 시작 Item은 시작점에, 마지막 Item은 끝점에 정렬되고 나머지 Items는 사이에 고르게 정렬됨	
- space-around: Items를 균등한 여백을 포함하여 정렬
```css
justify-content: 정렬방법;
```
![](https://images.velog.io/images/whdvkf92/post/e3e1603d-b8ab-42cc-a0f1-d0f055229d73/flex-7.JPG)

### align-content
교차 축(cross-axis)의 정렬 방법을 설정합니다.
주의할 점은 flex-wrap 속성을 통해 Items가 여러 줄(2줄 이상)이고 여백이 있을 경우만 사용할 수 있습니다.
- stretch: Container의 교차 축을 채우기 위해 Items를 늘림	stretch
- flex-start: Items를 시작점(flex-start)으로 정렬	
- flex-end: Items를 끝점(flex-end)으로 정렬	
- center: Items를 가운데 정렬	
- space-between: 시작 Item은 시작점에, 마지막 Item은 끝점에 정렬되고 나머지 Items는 사이에 고르게 정렬됨	
- space-around: Items를 균등한 여백을 포함하여 정렬
![](https://images.velog.io/images/whdvkf92/post/fcc5eab2-17b6-4ca4-9554-a9e7a5f3d52f/flex-8.JPG)

### align-items
교차 축(cross-axis)에서 Items의 정렬 방법을 설정합니다.
Items가 한 줄일 경우 많이 사용합니다.

주의할 점은 Items가 flex-wrap을 통해 여러 줄(2줄 이상)일 경우에는 align-content 속성이 우선합니다.
따라서 align-items를 사용하려면 align-content 속성을 기본값(stretch)으로 설정해야 합니다.
- stretch: Container의 교차 축을 채우기 위해 Items를 늘림	stretch
- flex-start: Items를 각 줄의 시작점(flex-start)으로 정렬	
- flex-end: Items를 각 줄의 끝점(flex-end)으로 정렬	
- center: Items를 가운데 정렬	
- baseline: Items를 문자 기준선에 정렬
![](https://images.velog.io/images/whdvkf92/post/a6db9357-ef96-4082-a5e8-0500ccaf2bfc/flex-9.JPG)

### Flex Items
Flex Items를 위한 속성들은 다음과 같습니다.

- order: Flex Item의 순서를 설정
- flex: flex-grow, flex-shrink, flex-basis의 단축 속성
- flex-grow: Flex Item의 증가 너비 비율을 설정
- flex-shrink: Flex Item의 감소 너비 비율을 설정
- flex-basis: Flex Item의 (공간 배분 전) 기본 너비 설정
- align-self: 교차 축(cross-axis)에서 Item의 정렬 방법을 설정

#### order
Item의 순서를 설정합니다.
Item에 숫자를 지정하고 숫자가 클수록 순서가 밀립니다.
음수가 허용됩니다.
```css
order: 순서;
```

#### flex
Item의 너비(증가, 감소, 기본)를 설정하는 단축 속성입니다.

- flex-grow:Item의 증가 너비 비율을 설정
- flex-shrink: Item의 감소 너비 비율을 설정
- flex-basis: Item의 (공간 배분 전) 기본 너비 설정
```css
flex: 증가너비 감소너비 기본너비;
```
```css
.item {
  flex: 1 1 20px;  /* 증가너비 감소너비 기본너비 */
  flex: 1 1;  /* 증가너비 감소너비 */
  flex: 1 20px;  /* 증가너비 기본너비 (단위를 사용하면 flex-basis가 적용됩니다) */
}
```
flex-grow를 제외한 개별 속성은 생략할 수 있습니다.
만약 flex: 1;로 작성하면 flex-grow: 1;과 같습니다.
그러면 나머지 속성은 생략했으니 기본값이 적용되어 flex-shrink: 1;, flex-basis: auto;가 되겠죠?
즉 flex: 1; 혹은 flex: 1 1;은 flex: 1 1 auto;와 같다고 볼 수 있습니다만 그렇지 않습니다.

flex-basis의 기본값은 auto입니다만 단축 속성인 flex에서 그 값을 생략할 경우 0이 적용됩니다.
다시 정리하면 flex: 1; 혹은 flex: 1 1;은 flex: 1 1 0;이 된다는 것입니다.
이 부분을 기억하지 않으면 엉뚱한 결과가 나올 수 있으니 주의합시다!

<br />

## MediaQuey
CSS Media Query는 예를 들어 "뷰포트가 480 픽셀보다 넓다."라고 여러분이 지정한 규칙에 브라우저 및 장치 환경이 일치하는 경우에만 CSS를 적용할 수 있는 방법을 제공합니다. 미디어 쿼리는 반응형 웹 디자인의 핵심 부분이다. 뷰포트의 크기에 따라 서로 다른 스크린을 생성할 수 있기 때문이다.

### 미디어 쿼리 기본
```md
@media media-type and (media-feature-rule) {
  /* CSS rules go here */
}
```

미디어 쿼리 구문의 구성 요소:
여기 코드가 어떤 미디어를 위한 것인지 브라우저에 알려주는 미디어 유형(예를 들어, 인쇄 또는 화면).
괄호로 묶은 씨에스에스 규칙이 적용되기 위해 전달되어야 하는 규칙 또는 조건문 격인 - - 미디어 표현식.
조건문을 통과하고 미디어 유형이 올바른 경우 적용되는 씨에스에스 규칙 집합.

### 미디어 기능 규칙
미디어 유형을 지정한 뒤에 규칙을 적용할 미디어 기능을 선정할 수 있습니다.

<br />

### 너비와 높이
반응형 디자인을(그리고 광범위한 브라우저 지원이 되도록) 만들기 위해 가장 자주 탐문하는 기능은 뷰포트 너비이며, min-width와 max-width, width 등의 미디어 기능을 활용하여 뷰포트가 특정 너비 이상 또는 이하인 경우 씨에스에스를 적용할 수 있습니다.

이러한 특징들은 다른 화면 크기에 반응하는 조판을 생성하는 데 사용됩니다. 예를 들어 뷰포트가 정확히 600픽셀인 경우 본문 색상을 빨간색으로 변경하려면 다음과 같은 미디어 쿼리를 사용합니다.
```md
@media screen and (width: 600px) {
    body {
        color: red;
    }
}
```
<br />

## Typography
자와 문단의 속성을 제어하며 다음과 같은 스타일을 사용한다.

(1) 스타일 종류

	1. 글자
	가. font-family
	나. font-size
	다. line-height
	라. font-weight
	마. font-style
	바. font-variant

	2. 문단
	가. text-align(인라인 요소의 가로정렬 셋팅)
	나. text-indent(들여쓰기)
	다. text-decoration(글자장식 밑줄)
	라. text-transform(대문자 소문자)
	마. vertical-align(인라인 요소의 수직위치 정렬)
	바. letter-spacing(자간)
	사. word-spacing(단어와 단어사이)
	아. white-space(공백문자처리)
	자. word-break(줄바꿈처리)
    
(2) font-family

- 웹페이지의 글꼴지정

- 상속되는 스타일

- 웹페이지의 대표폰트는 body요소에 글꼴 지정

(3) font-size

- 글자 크기를 지정하며 상대단위, 절대단위를 사용할 수 있음

- 글자크기도 상속되는 속성이며 시스템 대표 글자크기는 body속성에 지정

- 제목요소, 폼요소는 글자크기에 상속되지 않음
- 절대단위

	＊ px → 해상도 기준

	＊ % → 백분율 단위

	＊ em → 척도단위(기준이 되는 값을 1로 보고 그에 대한 배율을 적용)
    
    
    
(4) line-height

- 인라인 요소의 높이를 표현한다.

- 글자가 요소 높이의 중간에 위치하도록 하기 위해서 사용.

- line height 계산법

	(line-height) - (font-size) / 2 = 반행간(행간의 절반)

	반행간을 글자의 상단과 글자의 하단에 배치

	반행간+글자크기+반행간 = line-height

	(20-12)/2 = 4px

	4px + 12px + 4px = 20px
    
(5) font-weight

- 글자의 무게를 표현하며 normal, 100~900, bold 등을 사용한다.

- 제목 요소는 bold가 적용된 요소다.



(6) font-style

- 글자 스타일을 표현하며 italic, oblique를 표현한다. 

(7) font-variant

- 소문자크기의 글자를 대문자로 표현할 때, 영문에만 적용.

- 사용하는 값은 normal, small-caps을 적용한다.

(8) text-align

- 인라인 요소의 가로정렬을 표시

- 인라인 요소는 텍스트, 이미지, 폼요소

- 스타일은 인라인 요소를 감싸는 "블록" 요소에 작성

- 사용하는 값은 left, center, right, justify를 사용한다.

(9) text-decoration

- 글자장식을 표현한다.

- 사용하는 값은 underline(밑줄), over-line(윗줄), line-throught(취소선)을 사용한다.

(10) text-transform

- 소문자, 대문자 변환을 표현하며 영문에 적용

- 사용하는 값은 uppercase(대문자), lowercase(소문자) capitalize(첫글자만 대문자) 등이 있다.

(11) text-indent

- 들여쓰기 및 내어쓰기를 표현하며 양수값은 들여쓰기, 음수값은 내어쓰기를 한다.

- text-indent를 이용하는 경우는 주로 음수값 -9999px을 이용하여 스크린에서 텍스트를 감출 때 많이 사용한다.

(12) letter-spacing(자간), word-spacing

- 글자 및 단어 사이의 간격을 제어
- 음수 양수값을 입력하여 간격제어

(13) vertical-align

- 인라인 요소끼리의 수직위치 정렬 표현

- 사용하는 값은 baseline, top, middle, bottom 등이 있음

- 스타일은 블록요소 안의 인라인 요소에 적용

(14) List-style-type

- 목록기호 타입을 바꿀 수 있으며 다양한 기호설정이 가능하다.

- 기본값을 사용하는 경우는 거의 없으며 주로 배경이미지를 이용하여 목록기호를 표시하므로 리스트에서 제공하는 목록기호는 none으로 설정하여 보이지 않게 한다.

- 리스트 설정은 부모요소인 ul, ol 자식요소인 li 둘 중의 어느 곳에 작성하여도 상관없음. 그러나 일반적으로 li에 선언.

<br />

## Background
background 속성은 태그의 배경을 지정하는 속성으로, font 속성과 비슷하게 세부적인 속성들을 한번에 쓸 수 있는 속성입니다.

### background-color
배경색을 의미하며, 값은 color 속성의 포맷을 사용합니다.

### background-image
배경 이미지를 설정하며, 주로 이미지 경로를 지정하는 방식으로 사용합니다.
경로는 background-image: url("이미지 경로") 처럼 작성합니다.
특별한 점은 컨테이너의 크기와 상관없이 삽입된 background-image의 크기는 컨테이너에 맞춰 늘어나거나 줄어들지 않고 그대로 표시되며,
이미지 보다 컨테이너가 더 크다면 이미지는 반복되어 표시되게 됩니다.

### background-repeat(repeat, no-repeat)
background-image로 컨테이너보다 작은 이미지를 적용하면 이미지가 반복되어 출력됩니다.
이때 background-repeat 속성을 사용하면 반복여부를 지정 할 수 있습니다.

### background-position
일반적으로 background-image 는 왼쪽 위부터 이미지를 출력합니다.
background-position 속성을 사용하면 이미지의 좌표를 수정 할 수 있게 됩니다.
margin, padding 속성에서 지정했던 것과 비슷하게 띄어쓰기를 기준으로 x좌표, y좌표를 지정합니다.
픽셀 뿐만 아니라 left, top, center, bottom, right 등의 상수도 쓸 수 있습니다.

#### background-size(contain, cover, custom)
요소 배경 이미지의 크기를 설정합니다. 그대로 두거나, 늘리고 줄이거나, 공간에 맞출 수 있습니다.

<br />

## Transition
CSS 트랜지션은 CSS 속성을 변경할 때 애니메이션 속도를 조절하는 방법을 제공합니다. 속성 변경이 즉시 영향을 미치게 하는 대신, 그 속성의 변화가 일정 기간에 걸쳐 일어나도록 할 수 있습니다. 예를 들어, 여러분이 어떤 요소의 색상을 흰색에서 검은색으로 변경한다면, 변화는 대개 즉시 일어납니다. CSS 트랜지션을 이용하면, 모두 커스터마이즈 가능한 어떤 가속도 곡선을 따르는 시간 주기마다 변화가 일어납니다.

두 상태 사이의 트랜지션을 포함하는 애니메이션을 종종 암묵적 트랜지션이라고 부르는데, 이는 시작과 종료 상태 사이의 상태를 브라우저가 암묵적으로 정의하기 때문입니다.

## Transition CSS 속성
### transition-property
트랜지션을 적용해야 하는 CSS 속성의 이름 혹은 이름들을 명시합니다. 여기에 나열한 속성만 트랜지션하는 동안 움직입니다. 또한, 다른 모든 속성에 대한 변화는 보통 때와 같이 즉시 일어납니다.

### transition-duration
트랜지션이 일어나는 지속 시간을 명시합니다. 트랜지션 동안 모든 속성에 적용하는 단일 지속 시간을 명시하거나, 다른 주기로 각 속성이 트랜지션하게 하는 여러 지속 시간을 명시할 수 있습니다.

### transition-timing-function(ease-in, ease-out, ease-in-out, cubic-bezier())
속성의 중간값을 계산하는 방법을 정의하는 함수를 명시합니다. Timing functions는 트랜지션의 중간값을 계산하는 방법을 결정합니다. 대부분의 타이밍 함수는 큐빅 베이지어(cubic bezier)를 정의하는 네 점에 의해 정의되므로 상응하는 함수의 그래프로 제공해서 명시할 수 있습니다. Easing Functions Cheat Sheet에서 이징(easing, 역자주: 시간에 따른 파라미터 값의 변화율을 명시하는 함수)을 선택할 수도 있습니다.

### transition-delay
속성이 변한 시점과 트랜지션이 실제로 시작하는 사이에 기다리는 시간을 정의합니다.

<br />

## Animations
CSS3 애니메이션은 엘리먼트에 적용되는 CSS 스타일을 다른 CSS 스타일로 부드럽게 전환시켜 줍니다. 애니메이션은 애니메이션을 나타내는 CSS 스타일과 애니메이션의 중간 상태를 나타내는 키프레임들로 이루어집니다.

CSS 애니메이션은 기존에 사용되던 스크립트를 이용한 애니메이션 보다 다음 세 가지 이유에서 이점을 가집니다.

- 자바스크립트를 모르더라도 간단하게 애니메이션을 만들 수 있습니다.
- 자바스크립트를 이용한 애니메이션은 잘 만들어졌더라도 성능이 좋지 못할때가 있습니다. CSS 애니메이션은 frame-skipping 같은 여러 기술을 이용하여 최대한 부드럽게 렌더링됩니다.
- 브라우저는 애니메이션의 성능을 효율적으로 최적화할 수 있습니다. 예를 들어 현재 안보이는 엘리먼트에 대한 애니메이션은 업데이트 주기를 줄여 부하를 최소화할 수 있습니다.

## Animations 속성
### animation-delay
엘리먼트가 로드되고 나서 언제 애니메이션이 시작될지 지정합니다.

### animation-direction(alternate)
애니메이션이 종료되고 다시 처음부터 시작할지 역방향으로 진행할지 지정합니다.

### animation-duration
한 싸이클의 애니메이션이 얼마에 걸쳐 일어날지 지정합니다.

### animation-iteration-count
애니메이션이 몇 번 반복될지 지정합니다. infinite로 지정하여 무한히 반복할 수 있습니다.

### animation-name
이 애니메이션의 중간 상태를 지정합니다. 중간 상태는  @keyframes 규칙을 이용하여 기술합니다.

### animation-play-state
애니메이션을 멈추거나 다시 시작할 수 있습니다.

### animation-timing-function
중간 상태들의 전환을 어떤 시간간격으로 진행할지 지정합니다.

### animation-fill-mode
애니메이션이 시작되기 전이나 끝나고 난 후 어떤 값이 적용될지 지정합니다.

<br />

## Selectors
### 요소, 클래스, ID 선택자(Type, Class, ID Selector)
```css
요소 선택자
h1 {
}

클래스 선택자
.class {
}

Id 선택자
#id {
}
```

### Child, Descendant & Sibling Combinators
```css
Child
parenjt > child

Descendant
parent descendants

Sibling Combinators
check ~ check

check + check
```
### Structural Pseudo-classes
```css
element:first-child
element:last-child
element:nth-child(n)
```

### User Action Pseudo-classes
```css
element:hover
element:focus
element:active
```