# 제목(Header)
#은 HTML에서 h1와 같고, #이 늘어날 수록 h2,h3..태그가 된다.
즉, 마크다운은 HTML 언어로 변경되어 동작이 된돠는 것을 알 수 있다.

마크다운은 HTML, CSS와 같이 표준 언어가 아니기 때문에 환경에 따라 결과가 다르게 나올 수 있다.

# 제목 1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6


# 문장(Paragraph)
일반적인 문장은 HTML이 p 태그와
동일하게 동작한다.


# 줄바꿈(Line Break)
HTML에서 p 태그는 줄바꿈을 못한다.  
그래서 줄바꿈을 위해서는 br 태그를 사용해야하는데  
마크다운에서는 2번의 띄워쓰기 혹은 <br/>
원시 HTML을 활용하여 br태그를 사용해서 줄바꿈으로 인식하게 한다.


# 강조(Emphasis)
_이텔릭_  
_를 앞뒤로 사용 시, 이텔릭체로 작성

**두껍게**  
**을 앞뒤로 사용 시, 두껍게 글자가 작성됨.

**_이텔릭 + 두껍게_**  
이와 같이 복합적으로 2개의 글자체를 함께 사용 가능

~~취소선~~  
~~을 앞뒤로 사용 시, 취소선 사용됨.

<u>밑줄</u>  
마크다운 문법에서는 밑줄에 대해서 제공하지 않는다.  
하여, u 태그를 활용한다.  
HTML에서는 CSS를 활용해서 글자를 꾸미기 때문에 u라는 태그를 HTML상에서 써본적은 없을 것이다. (HTML에서 사용 권장 x)


# 목록(List)
1. 순서가 필요한 목록
1. 순서가 필요한 목록
1. 순서가 필요한 목록  

마크다운에서 HTML의 ol태그글 위와 같이 사용 가능하며,  
ol태그 밑에 li 태그는 위와 같이 숫자 1만 넣어주면 사용이 가능하다.
마크다운에서는 숫자를 순차적으로 넣지 않더라도 마크다운이 알아서 인식한다.

1. 순서가 필요한 목록
1. 순서가 필요한 목록
1. 순서가 필요한 목록
    1. 순서가 필요한 목록
    1. 순서가 필요한 목록
1. 순서가 필요한 목록

li 태그 밑에 하위 내용이 더 작성되는 경우에는 띄워쓰기 4번으로 작성 가능하다. (GITHUB상 들여쓰기 2번)


- 순서가 필요하지 않은 목록
- 순서가 필요하지 않은 목록
- 순서가 필요하지 않은 목록
    - 순서가 필요하지 않은 목록
    - 순서가 필요하지 않은 목록
        - 순서가 필요하지 않은 목록
- 순서가 필요하지 않은 목록


# 링크(Links)
<a href="https://google.com">GOOGLE</a>

[GOOGLE](https://google.com)

<a href="https://google.com" title="구글로 이동!">GOOGLE</a>

[GOOGLE](https://google.com "구글로 이동!")

<a href="https://google.com" title="구글로 이동!" target="_blank">GOOGLE</a>  
마크다운에서는 target="_blank" 은 제공하지 않는다.


# 이미지(Images)
![HEROPY](https://heropy.blog/css/images/logo.png)  
링크와 이미지 차이는 맨앞에 ! 외에는 문법이 같음.

[![HEROPY](https://heropy.blog/css/images/logo.png)  ](https://heropy.blog/)  
이렇게 링크에 글자를 이미지로 구성할 수도 있다.


# 인용문(BlockQuote)
> 인용문 : 남의 말이나 글에서 직접 또는 간접으로 따온 문장.  
> (네이버 국어 사전)

> 인용문을 작성하세요!
>> 중접된 인용문
>>> 중접된 인용문 1
>>>> 중접된 인용문 2
>>>>> 중접된 인용문 3


# 인라인(Inline) 코드 강조
CSS에서 `background` 혹은
`background-image` 속성으로 요소에 배경 이미지를 삽입할 수 있습니다.


# 블록(block) 코드 강조
```html
<a href="https://google.com" target="_blank">GOOGLE</a>
```

코드를 적용시키는 것이 아닌 문자로써 보여줄 때 활용할 수 있다.  
html이라는 문자를 붙임으로써 html코드로 인식하여 하이라이팅을 해준다.

```css
.list > li {
    position: absolute;
    top: 40px;
}
```

```javascript
function func() {
    var a = 'AAA';
    retunr a;
}
```

```bash
$ git commit -m 'Study Markdown'
```

```plaintext
동해물과 백두산이 마르고 닳도록
하느님이 보우하사 우리나라 만세
```
개발 언어를 사용하는 블록 코드 강조가 아니라면 plaintext를 활용하여 단순하게 텍스트만 블록 코드 강조로 출력할 수 있다.


# 표(Table)
html의 table태그.

CSS position 속성

값 | 의미 | 기본값
--|--|--
static | 요소의 배치 기준 없음 | O
relative | 요소의 자기 자신 기준 | X
absolute | 위치 상 부모 요소 | X
fixed | 뷰포트 | X

값 | 의미 | 기본값
--|:--:|--:
static | 요소의 배치 기준 없음 | O
relative | 요소의 자기 자신 기준 | X
absolute | 위치 상 부모 요소 | X
fixed | 뷰포트 | X

가운데 밑 우측 정렬 추가(기본 왼쪽 정렬)


# 원시 HTML(Raw HTML)
마크다운이라는 것은 어디까지나 브라우저에 출력이 되어야 하기 때문에 표준의 HTML로 변환이 된다.  
 (HTML로 변환이 되지만 마크다운 자체는 표준개념이 없어 사용하는 환경에 따라 다르게 출력될 수 있다.)

마크다운은 결국에는 HTML로 변환되기 때문에 변환되기 전에도 마크다운 문법 내부에서 HTML 문법을 그대로 사용할 수 있다.  
(이를 원시 HTML이라고 한다.)

동해물과 <u>백두산이</u> 마르고 닳도록<br/>
하느님이 보우하사 우리나라 만세

```plaintext
밑줄에 대해서는 일반적으로 아래와 같이 CSS를 활용해야하나, 마크다운은 간결한 문법을 지향하기 때문에 u태그를 쓰기도 한다.
```

동해물과 <span style="text-decoration: underline;">백두산이</span> 마르고 닳도록<br/>
하느님이 보우하사 우리나라 만세


# 수평선(Horizontal RUle)

---

***

___




