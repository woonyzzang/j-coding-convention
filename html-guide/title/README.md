# title
> 각 페이지마다 서로 다른 규칙으로 사용중인 문서 제목 (title 요소) 규칙을 일관성 있게 일원화함으로써, 서비스 통일성을 및 검색 엔진에 대한 최적화를 높인다. 또한 문서 제목에 컨텐츠 제목을 포함시킴으로써, 외부

검색서비스에서 해당 컨텐츠의 노출이 더 용이해진다.

## 기본 규칙
``` html
<title>@컨텐츠 제목 &gt; @하위섹션명 : @서비스명</title>
```

## 문서제목 기본 요소
**@서비스명**
* 브랜드 서비스명

**컨텐츠 제목**
* 서비스에서 제공하는 컨텐츠의 제목

**하위 섹션명**
* 하나의 서비스내 하위 섹션명 (보통 서비스별 GNB에서 TAB으로 표현되는 구분)

## 각 요소별 상세규칙
**서비스 명**
* 모든 서비스는 문서 제목에 서비스명을 표기하는 것을 원칙으로 한다.
* 서비스명은 문서 제목에서 가장 뒷부분에 위치한다.

``` html
<title>Google</title>
```

**컨텐츠 제목**
* 하나의 컨텐츠를 대표하는 페이지의 경우, 반드시 해당 컨텐츠 제목을 문서 제목에 표기한다.
* 컨텐츠 제목은 문서 제목에서 가장 앞부분에 위치한다.
* 컨텐츠 제목과 서비스명 간의 구분자는 반드시 `:` 기호를 사용한다.
* 컨텐츠 제목의 특수기호가 들어갈시 엔티티코드로 변환가능한 기호는 반드시 escape 되어야 한다.

``` html
<title>Web&47;Mobile Integration : Google</title>
```

**하위 섹션명**
* 하위섹션명은 서비스명 앞에 표기한다.
* 하위섹션명의 구분자는 `>` (`&gt;`) 를 사용한다.
* 하위섹션명은 필수 요소는 아니다.

``` html
<title>Web&#47;Mobile Integration &gt; Overview : Google</title>
<title>Web&#47;Mobile Integration &gt; Web : Google</title>
<title>Web&#47;Mobile Integration &gt; Mobile : Google</title>
```