---
title: "변수"
subtitle: "변수 종류"
layout: single
permalink: /javascript/
tag: javascript
author_profile: false
comments: true
toc: true
---

## var, let , const의 차이
- ### var (변수 재선언 가능)
```javascript
    var variable = "변수선언함";
    console.log(variable); //변수선언함

    var variable = "또 변수선언함";
    console.log(variable); //또 변수선언함
```
- ### let (변수 재선언 불가능, 재할당 가능)
```javascript
    let variable = "변수선언함";
    console.log(variable); // 변수선언함

    variable = "변수재할당함";`
    console.log(variable); // 변수재할당함

    let variable = "변수 재선언함" // ERROR
```
- ### const (변수 재선언 불가능, 재할당 불가능)
```javascript
    const variable = "변수선언함";
    console.log(variable); //변수선언함

    variable = "변수재할당함"; //ERROR
    
    const variable = "변수 또 선언함"; // ERROR
```

    




