---
title: "[Markdown] 마크다운 기초 3 - 단락("
excerpt: ""

categories:
    - Markdown
tags:
    - Markdown
    - md
last_modified_at: 2022-11-25 21:12:18 +0900
---



# 7 단락(Paragraphs)


## 문단 나눔(hard breaks)과 줄 나눔(soft breaks)
줄바꿈을 하고 싶다면 마크다운은 단순히 하나의 직선으로 렌더링 합니다.
```
나는 나 자신과 모순되는가?
그렇다면 아주 잘되었다… 나는 나 자신과 모순이다,
(나는 크다… 나는 다량의 것을 품고 있다.)
```

아래와 같이 개행을 넣으면 결합이 깨지게 됩니다. 
```
나는 나 자신과 모순되는가?

그렇다면 아주 잘되었다… 나는 나 자신과 모순이다,

(나는 크다… 나는 다량의 것을 품고 있다.)
```

위와 같은 방법은 문단 나눔(hard breaks)라고 부릅니다.   
위에서 요구하는 것은 soft breaks 입니다.  

각 줄의 끝에 2번의 공백(스페이스)를 넣음으로 줄 나눔을 할 수 있습니다. 

```
나는 나 자신과 모순되는가?··
그렇다면 아주 잘되었다… 나는 나 자신과 모순이다,··
(나는 크다… 나는 다량의 것을 품고 있다.)
```

```
// 문제 
시가 올바르게 렌더링 되도록 필요한 공백을 넣어보세요. 

// 주어진 코드 
We pictured the meek mild creatures where
They dwelt in their strawy pen,
Nor did it occur to one of us there
To doubt they were kneeling then.


// 정답 코드 
We pictured the meek mild creatures where  
They dwelt in their strawy pen,  
Nor did it occur to one of us there  
To doubt they were kneeling then.  
```

We pictured the meek mild creatures where  
They dwelt in their strawy pen,  
Nor did it occur to one of us there  
To doubt they were kneeling then.


## 리스트 내에서의 단락을 구성 
일반적인 용도는 리스트 내에서 단락을 포맷하는 것입니다. 

```
// 문제 
단락 나눔(hard breaks)대신에 줄 나눔(soft breaks)를 사용하여 하위 단락을 구성해보세요. 

// 주어진 코드
1. Crack three eggs over a bowl.

 Now, you're going to want to crack the eggs in such a way that you don't make a mess.

 If you _do_ make a mess, use a towel to clean it up!

2. Pour a gallon of milk into the bowl.

 Basically, take the same guidance as above: don't be messy, but if you are, clean it up!
// 정답 코드 
```
