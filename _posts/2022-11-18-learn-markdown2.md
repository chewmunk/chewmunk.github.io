---
title: "[Markdown] 마크다운 기초 정리 2 - 이미지(images), 인용문(Blockquotes), 리스트(Lists)"
excerpt: ""

categories:
    - Markdown
tags:
    - Markdown
    - md
last_modified_at: 2022-11-18 00:00:40 +0900
---


# 4 이미지(Image)

마크다운에서 링크를 사용할 줄 안다면, 이미지로 사용할 수 있습니다.  
문법이 거의 동일합니다.  
  
이미지 또한 두가지 타입이 존재합니다.  
링크처럼 두 타입 모두 렌더링 되는 방식은 같습니다.  
  
링크와 이미지의 차이는 이미지는 앞에 느낌표를 사용합니다 (!)
  
  
## 4.1 인라인 이미지 링크

인라인 이미지 링크를 사용하기 위해 느낌표를 입력하고 ! 대괄호로 [] 대체 텍스트를 감싼 다음, 소괄호 () 로 링크를 감싸면 됩니다.  
  
느낌표! -> 대괄호[] -> 소괄호()  

예를 들어, https://octodex.github.com/images/bannekat.png에 대한 이미지 링크와  Benjamin Bannekat란 대체 텍스트를 생성하려 할 때, 여러분은 마크다운에서 이렇게 사용하시면 됩니다
```
![Benjamin Bannekat](https://octode.github.com/images/bannekat.png)
```

![Benjamin Bannekat](https://octodex.github.com/images/bannekat.png)


```
// 문제 
이미지 링크로 바꾼 후, 대체 텍스트를 "A pretty tiger"로 바꿔보세요


// 주어진 코드 
[](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)

// 정답 코드

![A pretty tiger](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)


```

![A pretty tiger](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)


## 4.2 참조 이미지 링크

문장 앞에 느낌표를 사용한 후 대체 텍스트에 대괄호를 사용하고, 이미지 태크에 대괄호를 사용하면된다.  
  
```
![텍스트][태그이름]
![The founding father][Father]
```

마크 다운 페이지 맨 하단에는 이미지 태그를 정의 하면된다. 
  
```
// 링크 변수라고 생각하면 된다. 

[태그이름]: 링크주소 
[Father]: http://octodex.github.com/images/founding-father.jpg.
```

```
// 문제 
우리는 참조 이미지를 사용하고자 합니다. 지난 강의처럼 이것을 해결해야 다음 강의로 넘어가는 것 아시죠? "Black"이란 이미지 태그로 https://upload.wikimedia.org/wikipedia/commons/a/a3/81_INF_DIV_SSI.jpg 이미지 링크를 만들어주세요. 두번째 이미지 링크는 http://icons.iconarchive.com/icons/google/noto-emoji-animals-nature/256/22221-cat-icon.png 이미지 링크로 만들어주세요.

// 주어진 코드 
[Black cat][]

[Orange cat][Orange]

[Black]: https://upload.wikimedia.org/wikipedia/commons/a/a3/81_INF_DIV_SSI.jpg


// 정답 코드 
[Black cat][Black]

[Orange cat][Orange]

[Black]: https://upload.wikimedia.org/wikipedia/commons/a/a3/81_INF_DIV_SSI.jpg
[Orange]: http://icons.iconarchive.com/icons/google/noto-emoji-animals-nature/256/22221-cat-icon.png


```

[Black cat][Black]

[Orange cat][Orange]

[Black]: https://upload.wikimedia.org/wikipedia/commons/a/a3/81_INF_DIV_SSI.jpg
[Orange]: http://icons.iconarchive.com/icons/google/noto-emoji-animals-nature/256/22221-cat-icon.png

# 5 인용문 (Blockquotes)

인용문은 > 을 말하는 것이고   
인용구는 ""가 있는 문구를 말하는 것이다. 

인용문을 언급하거나 잡지 기사의 인용문을 디자인해야 한다면, 마크다운의 인용문을(blockquote) 구문이 유용할 것입니다.  

인용문을 사용하기 위해서는 ~보다 큰 의미의 캐럿 기고 > 만 붙여주면 됩니다. 

```
> "잠시 후 그는 맨발로 양말을 주모니에 넣고 캔버스 신발이 어깨 위로 매듭지어져 있는 끈에 매달려 있었고
바위들 사이에서 제 담에서 뾰족한 소금 먹은 막대기를 골라 방파제의 비탈을 기어내려갔다."

```

> "잠시 후 그는 맨발로 양말을 주모니에 넣고 캔버스 신발이 어깨 위로 매듭지어져 있는 끈에 매달려 있었고
바위들 사이에서 제 담에서 뾰족한 소금 먹은 막대기를 골라 방파제의 비탈을 기어내려갔다."


## 5.1 인용문 연습하기 1 

```
// 문제
아래 입력 창에서, 인용구에 인용문을 적용시켜보세요.

// 주어진 코드
I read this interesting quote the other day:

"Her eyes had called him and his soul had leaped at the call. To live, to err, to fall, to triumph, to recreate life out of life!"

// 정답 코드 
I read this interesting quote the other day:

> "Her eyes had called him and his soul had leaped at the call. To live, to err, to fall, to triumph, to recreate life out of life!"
```

## 5.2 여러 줄에 인용문 적용하기 = 인용문 그룹화 시키기

인용문의 각 줄에 캐럿 기호를 배치할 수도 있습니다. 인용구가 여러 단락에 이르는 경우 특히 유용합니다. 


```
> 그의 말은 그 자신의 천성적으로 어떤 깊은 화음에 부딪친 것 같았다. 그는 자기 자신에 대해, 있는 그대로 또는 되고 싶은 대로 말하였는가? 
스티븐은 잠시 동안 말없이 그의 얼굴을 지켜보았다. 차가운 슬픔이 그곳에 있었다. 그는 자신에 대해, 그가 두려워하는 외로움에 대해 이야기했다.
>
> —누구한테 말하는 거야? 스티븐이 길게 물었다.
>
> 크랜리는 대답하지 않았다.
```

> 그의 말은 그 자신의 천성적으로 어떤 깊은 화음에 부딪친 것 같았다. 그는 자기 자신에 대해, 있는 그대로 또는 되고 싶은 대로 말하였는가? 
스티븐은 잠시 동안 말없이 그의 얼굴을 지켜보았다. 차가운 슬픔이 그곳에 있었다. 그는 자신에 대해, 그가 두려워하는 외로움에 대해 이야기했다.
>
> —누구한테 말하는 거야? 스티븐이 길게 물었다.
>
> 크랜리는 대답하지 않았다.
  

빈 줄에도 캐럿 기호를 포함시켜야한다. 그러면 전체 인용문들이 다 함께 그룹화 됩니다.  


```
// 문제 
각 라인에 캐럿 기호를 넣어서 모든 인용할 부분을 하나의 인용문으로 만들어보세요.


// 주어진 코드
>Once upon a time and a very good time it was there was a moocow coming down along the road and this moocow that was coming down along the road met a nicens little boy named baby tuckoo...

His father told him that story: his father looked at him through a glass: he had a hairy face.

He was baby tuckoo. The moocow came down the road where Betty Byrne lived: she sold lemon platt.

// 정답 코드 

> Once upon a time and a very good time it was there was a moocow coming down along the road and this moocow that was coming down along the road met a nicens little boy named baby tuckoo...
> 
> His father told him that story: his father looked at him through a glass: he had a hairy face.
> 
> He was baby tuckoo. The moocow came down the road where Betty Byrne lived: she sold lemon platt.
> 
```


## 5.3 인용문 내에 이탤릭체 넣어보기 

인용문 내에서 이탤릭체, 이미지, 링크와 같은 다른 마크다운 요소도 사용할 수 있습니다.  
  
```
// 문제
불어에 이탤릭체를 적용시켜보세요(느낌표는 포함하지 말아주세요) 또한 전체 인용 부분에 인용문을 적용시켜보세요.

// 주어진 코드
He left her quickly, fearing that her intimacy might turn to jibing and wishing to be out of the way before she offered her ware to another, a tourist from England or a student of Trinity. Grafton Street, along which he walked, prolonged that moment of discouraged poverty. In the roadway at the head of the street a slab was set to the memory of Wolfe Tone and he remembered having been present with his father at its laying. He remembered with bitterness that scene of tawdry tribute. There were four French delegates in a brake and one, a plump smiling young man, held, wedged on a stick, a card on which were printed the words: VIVE L'IRLANDE!


// 정답 코드 
> He left her quickly, fearing that her intimacy might turn to jibing and wishing to be out of the way before she offered her ware to another, a tourist from England or a student of Trinity. Grafton Street, along which he walked, prolonged that moment of discouraged poverty. In the roadway at the head of the street a slab was set to the memory of Wolfe Tone and he remembered having been present with his father at its laying. He remembered with bitterness that scene of tawdry tribute. There were four French delegates in a brake and one, a plump smiling young man, held, wedged on a stick, a card on which were printed the words: _VIVE L'IRLANDE_!
```

# 6. 리스트(Lists)

리스트 타입은 보통 2가지가 존재합니다.  
순서가 매겨지지 않는 것(unordered)과 순서가 매겨진 것(ordered)입니다.  
별표(*)로 된 리스트와 숫자로 된 리스트가 존재한다고 말씀드리는게 더 적절합니다.  


## 6.1. 순서가 매겨지지 않은 리스트(unordered lists)

순서개 매겨지지 않은 리스트를 상성하기 위해서는 각 리스트의 각 항목에 별표를 앞에 붙여주면 됩니다.
* 우유
* 계란
* 연어
* 버터

```
// 문제
쉼표 기준으로 각 단어를 순서가 매겨지지 않은 리스트로 바꿔보세요.

// 주어진 코드
Flour, Cheese, Tomatoes

// 정답 코드 
* Flour
* Cheese
* Tomatoes
```

## 6.2 순서가 매겨진 리스트(ordered list)
  
순서가 매겨진 리스트에 대해 알아보자. 
  
순서가 매겨진 리스트는 별표대신 숫자를 붙여줍니다. 

1. 보울 위에 계란 세 개를 깨뜨린다
2. 우유 3.7L를 그릇에 붓는다
3. 버터를 힘차게 연어를 문지른다
4. 연어를 우유,계란을 쏟은 그릇에 넣는다

```
// 문제
요리법의 순서를 순서가 매겨진 리스트로 바꾸어보세요.

// 주어진 코드
Cut the cheese, Slice the tomatoes, Rub the tomatoes in flour

// 정답 코드 
1. Cut the cheese
2. Slice the tomatoes
3. Rub the tomatoes in flour
```

## 6.3 리스트 안에 이탤릭체 넣어보기 

리스트 안에 이탤릭체, 볼드체, 링크를 추가할 수 있습니다.  

```
// 문제
식물의 라인어 이름을 이탤릭체로 바꿔보세요.

// 주어진 코드 
* Azalea (Ericaceae Rhododendron)
* Chrysanthemum (Anthemideae Chrysanthemum)
* Dahlia (Coreopsideae Dahlia)

// 정답 코드 
* Azalea (_Ericaceae Rhododendron_)
* Chrysanthemum (_Anthemideae Chrysanthemum_)
* Dahlia (_Coreopsideae Dahlia_)

```


## 6.4 깊이있는 리스트 만들기 

좀 더 깊이 있는 리스트를 만들거나, 리스트에 다른 리스트를 겹쳐서 만들 수도 있습니다. 

앞의 항목보다 공백 한칸을 별표 앞에 더 들여놓으면 됩니다. 

* 틴틴
 * 기자
 * 얼간이 같은 주황색 머리
 * 세상에서 제일 멋진 개와 친구들
* 햅덕
 * 선장
 * 멋진 턱수염
 * 위스키 좋아함
   * 아마 스카치도?


```
* 틴틴
 * 기자
 * 얼간이 같은 주황색 머리
 * 세상에서 제일 멋진 개와 친구들
* 햅덕
 * 선장
 * 멋진 턱수염
 * 위스키 좋아함
   * 아마 스카치도?
```


```
// 문제
인물의 특징을 하위 목록으로 만들어보세요.

// 주어진 코드 
* Calculus, A professor, Has no hair, Often wears green
* Castafiore, An opera singer, Has white hair, Is possibly mentally unwell

// 정답 코드 
* Calculus
 * A professor
 * Has no hair
 * Often wears green
* Castafiore
 * An opera singer
 * Has white hair
 * Is possibly mentally unwell

```

무한적 하위 리스트를 추가할 수 있지만, 대개는 3단계까지만 사용하는 것이 좋습니다.  
그렇지 않으면, 텍스트는 엉망진창이 될 것입니다.  



## 6.5 단락을 다루는 방법 
