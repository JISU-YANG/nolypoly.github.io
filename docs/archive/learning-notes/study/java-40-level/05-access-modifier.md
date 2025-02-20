---
layout: note_series
parent: Learning Notes
study: Java 40 Level
chapter: 5
title: Access Modifier
toc: true
reference:
  1:
    author: 한동석
    year: 2019
    platform: 코리아IT아카데미
    content: JAVA 단과 과정
    content-link:
  2:
    author: 전민균
    year: 2019
    platform: 코리아IT아카데미
    content: 웹 개발자 양성 과정
    content-link: 
---
### 접근 제한자 (Access Modifier)

접근 제한자는 생성된 객체의 변수와 메소드를 접근할 수 있는 범위를 정해준다.

---

### 접근 제한자 (Access Modifier)의 종류

- public
  - 모든 범위에서 접근이 가능하다.
- protected
  - (default)와 같으나 다른 패키지여도 확장(상속)관계이면 접근이 가능하다.
- (default)
  - 생략하여 사용한다.
  - 기본적으로 같은 패키지 안에 있는 Class라면 접근이 가능하다.
- private
  - 자기 클래스 내부(Member)에서만 접근이 가능하다.

---

### 접근 제한자 (Access Modifier)의 범위

|대상 Class|자기 Class|같은 Package|확장 (extends)|다른 Package|
|:--:|:--:|:--:|:--:|:--:|
|public|O|O|O|O|
|protected|O|O|O|X|
|(default)|O|O|<- O / X ->|X|
|private|O|X|X|X|
