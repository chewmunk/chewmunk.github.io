---
title: "[Markdown] 마크다운 기초 정리 1 - 이탤릭체, 볼드체, 헤더, 링크(inline link, reference link)"
excerpt: ""

categories:
    - Markdown
tags:
    - Markdown
    - md
last_modified_at: 2022-11-17 23:40:34 +0900
---

# 1. 이탤릭체와 볼드체(Italics and Bold)

마크다운은 일반 텍스트와 보이는 것이 크게 다르지 않지만, 좀 더 쉽게 볼 수 있도록 강조(highlighting)를 제공하고 있습니다.  


## 1.1 이탤릭체 사용 방법 
마크 다운으로 이탤릭체를 사용하기 위해서 여러분은 글자 바깥쪽에 밑줄(_)을 추가하면 됩니다. 예를 들어, _이것_ 은 이탤릭체가 됩니다. 
```
_이것_
```

## 1.2 볼드체 사용 방법
마크다운에서 볼드체를 사용하기 위해서, 글자의 바깥쪽에 별표(**)를 추가하면됩니다. **정말** 이런식으로요.
```
**정말**
```

## 1.3 이탤릭체와 볼드체 같이 사용하기 

볼드체(bold)와 이탤릭체(italics)를 모두 적용한 단어를 만들 것입니다.  
일반적으로 별표와 밑줄을 어느 순서로 배열하든지 상관없습니다.  
**_바깥쪽에_** 

```
**_바깥쪽에_**
```

# 2 헤더(Headers)

공지사항에 자주 사용되어 한 구획에 대한 이목을 끌도록 합니다.  
헤더는 한 구획에서 제목이나 부제로 사용됩니다. 

## 2.1 헤더의 종류 
헤더는 6가지 타입이 존재합니다. 사이즈 순으로 나열하겠습니다.

마크다운에서 헤더를 만들기 위해서는 마크(#)를 문단 앞에 사용하면됩니다.  
헤더 사이즈 크기만큼 해쉬 마크 갯수를 늘려 사용하면 됩니다.  
헤더 1을 사용하기 위해서는 (# 헤더 1)를 1개 사용할 수 있습니다.  
헤더 3을 사용하기 위해서는 해쉬 마크(### 헤더 3)를 3개 사용할 수 있습니다. 

```
// 문제 
각 헤더를 앎자은 사이즈로 만들어보세요.

// 주어진 코드
Header one
Header two
Header three
Header four
Header five
Header six

// 정답 코드 
# 이것은 헤더 1입니다.
## 이것은 헤더 2입니다.
### 이것은 헤더 3입니다.
#### 이것은 헤더 4입니다.
##### 이것은 헤더 5입니다.
###### 이것은 헤더 6입니다. 
```

## 2.2 헤더에 이탤릭체 입히기 
헤더에 볼드체(bold)를 입힐 순 없지만, 특정 단어에 이탤릭체는 사용할 수 있습니다.  
<!-- #### Colombian Symbolism in _One Hundred Years of Solitude_   -->

Here's some words about the book _One Hundred Years..._.

문제 
```js
// 문제
아래 입력 창에서 첫번째줄을 헤더 4로 책의 이름을 이탤릭체로 만들어보세요.
Colombian Symbolism in One Hundred Years of Solitude

// 주어진 코드
Here's some words about the book _One Hundred Years..._.

// 정답 코드
#### Colombian Symbolism in _One Hundred Years of Solitude_

Here's some words about the book _One Hundred Years..._.
```  

# 3. 링크(Links) 

다른 웹사이트로 이동할 수 있는 링크에 대해서 배울 것입니다.

마크다운에는 2가지 링크 유형이 있지만, 2가지 링크 유형 모두 정확히 같은 방식으로 랜더링됩니다.

## 3.1 인라인 링크(Inline Link) 
첫 번째 링크 스타일은 인라인 링크 스타일 이라고 부릅니다.  
인라인 링크를 만들기 위해서는 텍스트를 대괄호[]로 감싼 후 링크할 주소를 소괄호()로 감싸면 됩니다.  

쉽게 외우기 

대괄호 안에는 텍스트, 소괄호 안에는 링크. 대(텍스트) -> 소(링크)


### 3.1.1 링크 만들기
예제 코드 1  
[Github 방문!](www.github.com)  
[Search for it.](www.google.com)

```
// 문제 
Search for it 란 텍스트에 www.google.com로 링크되도록 링크를 만들어보세요.

// 주어진 코드
Search for it. 

// 정답 코드
[Github 방문!](www.github.com)
[Search for it.](www.google.com)
```  

### 3.1.2 링크된 텍스트에 볼드체 추가하기
예제 코드 2  

[You're **really, really** going to want to see this.](www.dailykitten.com)

```
// 문제 
아래 입력창에서 "really, really"를 볼드체로, 전체 문장이 www.dailykitten.com로 링크 되도록 만들어보세요. 볼드체가 링크 대괄호 안에서 발생하는지 확인해 보세요.

// 주어진 코드 
You're really, really going to want to see this.

// 정답 코드 
[You're **really, really** going to want to see this.](www.dailykitten.com)
```

### 3.1.3 헤더에 링크 만들기 

```
// 문제
아래 문장을 헤더 4로 만들고 the BBC를 www.bbc.com/news로 링크되도록 만들어보세요.

// 주어진 코드
The Latest News from the BBC

// 정답 코드 
#### The Latest News from [the BBC](www.bbc.com/news)
```



## 3.2 참조 링크 
참조 링크는 실제로 문서 내의 다른 위치에 대한 참조를 나타냅니다.  
여기 [태그 1][참조 링크1]가 있습니다.  
여기 [태그 1][참조 링크2]가 있습니다.  
앗, [태그 3][참조 링크1]도 있었네요.  

[참조 링크1]: https://www.github.com
[참조 링크2]: https://www.google.com

```
// 예제
여기 [태그 1][참조 링크1]가 있습니다.  
여기 [태그 1][참조 링크2]가 있습니다.  
앗, [태그 3][참조 링크1]도 있었네요.  

[참조 링크1]: www.github.com
[참조 링크2]: www.google.com
```

참조는 위에서 두버째로 나타내는 대괄호들을 의미합니다.   
\[참조 링크1\]와 \[참조 링크2\]  

이 대괄호들은 마크다운 문서 하단에 외부 웹사이트에 대한 적절한 링크로 정의됩니다. 
참조 링크 스타일의 장점은 같은 장소에 대한 다중 링크는 한 번만 업데이트하면 된다든 것입니다.  
예를 들어 \[참조 링크1\] 링크를 모두 다른 사이트로 이동시키로 했다면 우리는 하나의 참조 링크만 변경하면 됩니다.  

렌더링된 마크다운에서는 참조 링크가 나타나지 않습니다.
참조 링크를 정의하는 방법은 묶은 참조 태그를 작성하고 그 다음에 콜론, 그 다음에 링크할 주소를 작성하면 됩니다.  

```
// 문제
첫 번째 참조 태그를 "a fun place"로 정의하고, www.zombo.com에 연결하세요.  
두 번째 참조 태그 "another fun place"를 www.stumbleupon.com로 링크되도록 만들어보세요.

// 주어진 코드 
Do you want to [see something fun][]?
Well, do I have [the website for you][another fun place]!

// 정답 코드 
Do you want to [see something fun][a fun place]?
Well, do I have [the website for you][another fun place]!

[a fun place]: www.zombo.com
[another fun place]: www.stumbleupon.com
```

Do you want to [see something fun][a fun place]?  
Well, do I have [the website for you][another fun place]!  

> 쉽게 외우는 방법

첫대괄호 텍스트, 두번째 대괄호 참조변수
\[텍스트\]\[참조변수\]  
\[참조변수\]\: 링크주소

링크 주소를 변경하고 싶을때 정의된 참조 변수만 변경하면된다.  
참조 링크라고 부르지만, 변수와 같은 역할을 하기에 참조 변수라 이름을 붙이도록 하겠다.  







[a fun place]: https://www.zombo.com
[another fun place]: https://www.stumbleupon.com