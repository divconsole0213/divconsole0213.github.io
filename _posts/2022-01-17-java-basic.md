---
title: "변수"
layout: "single"
categories: "JAVA"
tags: "자바"
author_profile: true
comments: true
---

### 변수 종류
클래스 영역에 위치하는 변수
  -클래스 변수 : 클래스에 메모리가 올라갈때
  -인스턴스 변수 : 인스턴스가 생성되었을때 

클래스 영역 이외의 영역에 위치하는 변수
<div color ="red">('메소드, 생성자, 초기화 내부')<div>
 -<div color="red">지역 변수</div>: 변수 선언문이 수행되었을때
 - 지역변수의 생존범위: 

 <p> ex) public static void main(String[]args){
     variable a;
     method m(a){
     variable b;
      syso(<div color ="blue">method m은 ()내부의 a를 읽을 수있습니다 여기서 a는 전역변수(클래스 영역에 위치하는 변수)를 의미합니다./</div>
    <div color ="red">method m() {
          variable b는 method m(){}의 괄호바깥으로 나가면 운명을 다합니다 ㅠ,ㅠ</div>
      }  )       
     }

 }