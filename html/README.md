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
- [SEO](#seo)
  - [Title](#title)
  - [Metadata](#metadata)
  - [Open Graph](#open-graph)
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

## SEO

### Title

- 분류 : Metadata Content
- 문맥 : Head 요소의 자식
- 콘텐츠 모델 :텍스트, 공백만으로 구성할 수 없음
- 태그 생략 : 시작 태그와 종료 태그 생략 불가능

페이지 타이틀을 통해 요청한 페이지에 접속했는지 빠르게 판단할 수 있으며, 화면 낭독기 사용자는 웹 페이지 접속 시 페이지 타이틀을 음성으로 전달 받는다  
그리고 구체적인 키워드를 앞으로 배치하고, 가능한 짧게 작성하는 것이 좋다

#### 작성 가이드

- 대시(-), 파이프(|), 콜론(:)을 추천

```text
Page title - Site name
Page title | Site name
Page title : Site name
```

### Metadata

- html, head

```html
<html lang="ko">
<head>
  <meta charset="utf-8">
  <meta name="description" content="A description of the page">
  <meta name="keywords" content="webtoon, audit"> <!-- 구글은 어뷰징으로 문제로 인해 판단하지 않는다 -->
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Page title - Site name</title>
</head>
</html>
```

#### Naver 연관채널

JSON-LD 형식 구현 예제

```html
<script type="application/ld_json">
{
  "@context": "http://schema.org",
  "@type": "Person",
  "name": "My Site Name",
  "url": "http://www.mysite.com",
  "sameAs": [
    "https://www.facebook.com/myfacebook",
    "http://blog.naver.com/myblog",
    "http://storefarm.naver.com/mystore"
  ]
}
</script>
```

Microdata 형식 구현 예제

```html
<span itemscope="" itemtype="http://schema.org/Organization">
  <link itemprop="url" href="http://www.mysite.com">
  <a itemprop="sameAs" href="https://www.facebook.com/myfacebook"></a>
  <a itemprop="sameAs" href="http://blog.naver.com/myblog"></a>
  <a itemprop="sameAs" href="http://storefarm.naver.com/mystore"></a>
</span>
```

- https://searchadvisor.naver.com/guide/structured-data-channel
- https://schema.org/docs/gs.html

#### Open Graph

Facebook

```html
<meta property="og:url" content="http://www.nytimes.com/2015/02/19/arts/international/when-great-minds-dont-think-alike.html" />
<meta property="og:type" content="article" />
<meta property="og:title" content="When Great Minds Don’t Think Alike" />
<meta property="og:description" content="How much does culture influence creative thinking?" />
<meta property="og:image" content="http://static01.nyt.com/images/2015/02/19/arts/international/19iht-btnumbers19A/19iht-btnumbers19A-facebookJumbo-v2.jpg" />
```

- https://developers.facebook.com/docs/sharing/webmasters/
- https://developers.facebook.com/tools/debug/

Twitter

```html
<meta name="twitter:card" content="summary">
<meta name="twitter:title" content="">
<meta name="twitter:description" content="">
<meta name="twitter:image" content="">
```

- https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/markup

## References

- [https://html.spec.whatwg.org/](https://html.spec.whatwg.org/)
- [https://caniuse.com/](https://caniuse.com/)
