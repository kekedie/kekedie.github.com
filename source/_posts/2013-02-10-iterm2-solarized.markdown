---
layout: post
title: "iTerm2 Solarized 테마설정"
date: 2013-02-10 19:08
comments: true
categories: Development
---
보기 좋은 떡이 먹기도 좋다고 요즘 각종 툴에 테마 설정을 이것저것 찾아 보던 중에 발견한 **[Solarized](http://ethanschoonover.com/solarized)**.
```
git clone git://github.com/altercation/solarized.git
tree solarized/iterm2-colors-solarized 
solarized/iterm2-colors-solarized
├── README.md
├── Solarized\ Dark.itermcolors
└── Solarized\ Light.itermcolors
```
**[github](git clone git://github.com/altercation/solarized.git
)**저장소에서 `Solarized`테마를 다운로드 받고 **iTerm2 > Preferences > Profiles > Colors > Load Presets... > Import...** 에서 위에서 클론 받아온 파일을 임포트 해주면 끝.

개인적으로는 바탕화면이 어두운걸 선호해서 `Solarized Dark.itermcolors`를 임포트해서 사용중이다.
레포지토리에 보면 기타 다른 툴에서도 같은 테마를 적용할 수 있게 임포트 파일들이 준비 되어 있다. 아쉽게도 [Eclipse](http://www.eclipse.org)는 빠졌는데 (intelliJ는 있는데...) [Eclipse Color Theme](http://eclipsecolorthemes.org)에서 [검색](http://eclipsecolorthemes.org/?list=all&q=solarized)해보면 괜찮은 자료가 많이 올라와 있다.

