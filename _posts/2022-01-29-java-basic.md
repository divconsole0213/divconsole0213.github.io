---
title: "casting 형변환"
layout: single
tag: java
categories: java
author_profile: false
comments: true
toc: true
---
## casting이란 

### 형변환
- 상속관계에 있는 부모와 자식 클래스 간에는 서로 간의 형변환이 가능하다.

### upcasting
- 자식 클래스가 부모클래스의 타입으로 캐스팅됨

### downcasting
- 부모클래스가 자식 클래스의 타입으로 캐스팅됨

#### 예시 
```java
package upcasting;

public class Couple {
	

	private String dadBloodType = "ao";
	private String momBloodType = "bo";
	
	
	public Couple() {
 this.dadBloodType = dadBloodType;
 this.momBloodType = momBloodType;
	}


	public String getMomBloodType() {
		return momBloodType;
	}

public String getDadBloodType() {
		return dadBloodType;
	}


//상속에 대한 설명이다.
//부부가 있다.
//아빠 혈액형은 a형
//엄마 혈핵형은 b형 
}

```
```java
package upcasting;

public class Child  extends Couple{
  
	private String ability;
	
	public void ability() {
	   ability = "피아노를 잘친다.";
	   System.out.println(ability);
	}
	//자식을 낳았다
	//자식의 혈액형은 아빠와 엄마에게 물려받을 것 이다.
	//자식은 피아노치는 능력을 타고났다
	//자식은 부모에게 피아노 치는 능력을 되물려 줄수 있을까? 
    
}

```
```java
package upcasting;

public class Heridity {

	public static void main(String[] args) {

		Couple couple_ = new Couple(); // 커플을 불러옵니다.
		Couple couple_child = new Child(); .
        Child child = new Child();// 커플이 낳은 자식도 불러옵니다.
        
		String dadBloodT_ = couple_.getDadBloodType();
		String momBloodT_ = couple_.getMomBloodType();
		String childBloodT_;
		String[] coupleBloodT_ = { dadBloodT_, momBloodT_ };

		int random = (int) (Math.random() * coupleBloodT_.length);
		System.out.println(random);
		
		  if(random == 0) { 
			  childBloodT_ = couple_child.getDadBloodType(); 
			  System.out.println(childBloodT_);
			  
		  }else {
			  childBloodT_ = couple_child.getMomBloodType();
		      System.out.println(childBloodT_);
		  }
		  
		  //부모는 자식의 피아노 능력을 물려받을 수 있을까요?
		  
		  couple_.ability(); //The method ability() is undefined for the type Couple
		  couple_child.ability();
		   //add cass to_Child  ==>  down cating
	      ((Child) couple_child).ability();  
		  child.ability();
		  }
}
```



