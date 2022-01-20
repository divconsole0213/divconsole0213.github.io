---
title: "변수"
subtitle: "변수 종류"
layout: single
permalink: /java/
tag: java
author_profile: false
comments: true
toc: true
---

&nbsp;클래스 영역에 위치하는 변수<br>
- 클래스 변수 : 클래스에 메모리가 올라갈때<br>
- 인스턴스 변수 : 인스턴스가 생성되었을때 <br>

&nbsp;클래스 영역 이외의 영역에 위치하는 변수(메소드, 생성자, 초기화 내부)<br>
- 지역 변수: 변수 선언문이 수행되었을때 <br>
&ensp;ex)&nbsp;지역변수의 생존범위&nbsp;: <br>

 ```java
   public class Test { 
     public static void main(String[] args) {
        int i = 0; 
          while(i<1) {
             int result = 100; 
             i++; 
             System.out.println(result); 
             } //result는 지역변수라서 }밖으로 나오면 생존하지 않는다.;
               //i는 {}전에 생성되었기 때문에 함수로 쓸 수 있고 
              } }

```

<p style="text-align"><img src="/assets/images/practice.png"></p>