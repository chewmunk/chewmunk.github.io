---
title: "[Markdown] 기초 정리 2 - 이미지, 인용문"
excerpt: "Markdown 기초 정리 2 - 이미지, 인용문"

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

