# HTML

## Table of Contents

- [Element Content Categories](#element-content-categories)
  - [Flow Content](#flow-content)
  - [Metadata Content](#metadata-content)
  - [Heading Content](#heading-content)
  - [Sectioning Content](#sectioning-content)
  - [Phrasing Content](#phrasing-content)
  - [Embedded Content](#embedded-content)
  - [Interactive Content](#interactive-content)
  - [Palpable Content](#palpable-content)
  - [Script Supporting Content](#script-supporting-content)
  - [Transparent Content Models](#transparent-content-models)
- [References](#references)

## Element Content Categories

- Flow Content
- Metadata Content
- Heading
- Sectioning
- Interactive
- Phrasing
- Embedded

### Flow Content

- body 에 포함 될 수 있는 모든 요소  
- base, styled, title 요소를 제외한 나머지 모든 요소

### Metadata Content

- 콘텐츠와 문서를 구조화 하는 요소를 의미  
- 다른 콘텐츠의 표시, 동작, 관계 등을 설정

### Heading Content

- heading tag(h1 - h6)

### Sectioning Content

- 문서의 개요를 형성
- 헤딩, 헤더, 푸터의 범위
- 각 섹셔닝 콘텐츠는 암시적인 개요를 형성
- 헤딩 콘텐츠를 함께 사용하면 명시적인 개요를 형성
- article, aside, nav, section

### Phrasing Content

- 구문 콘텐츠
- 단락을 형성하는 콘텐츠
- display: inline, inline-block, none

### Embedded Content

- 외부 자원을 참조하는 콘텐츠
- 모든 임베디드 콘텐츠는 구문 콘텐츠이다
- 외부 자원을 지원하지 않는 경우 대체 자원을 명시할 수 있다
- audio, canvas, embed, iframe, img, math, object, picture, svg, video

### Interactive Content

- 사용자와 상호 작용할 수 있는 콘텐츠

### Palpable Content

- 비어 있지 않은, 볼 수 있는 콘텐츠

### Script Supporting Content

- 렌더링하지 않지만 사용자에게 기능을 제공
- script, template

### Transparent Content Models

- 투명 콘켄츠 모델
- 부모의 콘텐츠 모델을 따른다
- 투명한 요소를 제거해도 부모와 자식 관계가 문법적으로 유효해야한다
- a, ins, del, object, video, audio, map, noscript, canvas

## CSS Attributes

- flex
- grid
- will-change
- filter
- aria

## References

- [https://html.spec.whatwg.org/](https://html.spec.whatwg.org/)
- [https://caniuse.com/](https://caniuse.com/)
