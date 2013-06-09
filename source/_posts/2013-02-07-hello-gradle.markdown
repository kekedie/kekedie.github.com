---
layout: post
title: "Hello Gradle!"
date: 2013-02-07 00:15
comments: true
categories: Gradle 
---
최근 프로젝트에서 사용중이였던 **Maven**을 **Gradle**로 이전하고 있는 중이다.
[Gradle사이트](http://www.gradle.org)에서 제공하고 있는 [Gradle User Guide](http://www.gradle.org/docs/current/userguide/userguide.html)를 보면서 테스트 중인데 **Maven**에서 프로젝트 의존성 문제로 골머리를 썪혔던 부분이 `settings.gradle`에 서브프로젝트 설정 한줄로 단번에 해결!
``` groovy
// 하위 디렉토리는 ':' 로 구분.
include "서브프로젝트1", "서브프로젝트2", "서브프로젝트3"
```
**Gradle**에서 `multi-project build` 설정은 정말 쉽다.
물론 각 서브프로젝트들도 `build.gradle`이 필요하지만 **Maven**에서 `xml`로 기술하던거랑은 비교할 수도 없이 간단하다. 
``` groovy
// 서브프로젝트1에서 서브프로젝트2와 의존관계가 있을 경우.
// ':'는 루트 프로젝트 디렉토리 인듯.
compile project(':서브프로젝트2')
```
서브프로젝트를 테스트 하거나 빌드를 할때도 루트프로젝트를 지정하지 않아도 알아서 `settings.gradle`을 찾아서 의존관계를 해결해 준다.

한마디로 빌드계에 **강남스타일**이라 할 수 있겠다 :)

