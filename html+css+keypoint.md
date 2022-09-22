// HTML 기초 //

- 웹 사이트에서 사용되는 문서.

- html, htm 확장자 사용

- 웹 편집기: 웹 문서 작성 / 웹 브라우저: 웹 문서 확인.


<!doctype html>: 문서 유형 선언문

<html>: 웹 문서 시작

<head>: 문서 정보 표시

<title>: 문서 제목 (검색 엔진에 중요)

<meta>: 문자 인코딩 (보통 <meta charset=”utf-8”> 사용)

<body>: 실제 브라우저에 표시될 내용


// 텍스트 태그 //

<h1>~<h6>: 제목 표시 (숫자가 작을수록 크기가 커짐)

<p>: 단락

<br>: 줄바꿈

<hr>: 수평줄

<blockquote>: 인용문 (블록 레벨 태그라서 들여쓰기)

<q>: 인용 내용 (인라인 레벨 태그라서 줄바꿈 X)

<pre>: 입력 그대로 출력 (접근성 고려 필요)

<strong>: 굵게 표시 (중요한 내용 강조)

<b>: 굵게 표시 (키워드처럼 단순 강조)

<em>: 이탤릭체 (특정 부분 강조)

<i>: 이탤릭체 (생각, 꿈, 기술적인 용어, 관용구 등)

<mark>: 형광펜 효과

<span>: 줄바꿈없이 일부 텍스트 묶기

<ruby>: 동아시아 글자 표시

<abbr>: 약자 표시

<cite>: 참고 내용 표시 (웹문서, 포스트 등)

<code>: 소스 코드

<kbd>: 키보드 입력, 음성 명령

<small>: 부가 정보 (작게 표시)

<sub>: 아래 첨자

<sup>: 위 첨자

<s>: 취소선

<u>: 밑줄

<ul>, <li>: 순서없는 목록 (css의 list-style-type에서 불릿 수정 가능)

<ol>, <li>: 순서있는 목록 (type 속성으로 숫자 종류 변경 가능)

<dl>, <dt>, <dd>: 설명 목록 (dl: 목록, dt: 제목, dd: 설명)

<table>, <tr>, <td>: 표 (tr:행, td:셀) table border=” ” : 셀 테두리

<th>: 제목 셀

<td(th) colspan = “ ”>: 행 합치기

<td(th) rowspan = “ ”>: 열 합치기

<caption>: 표 제목 (table 태그 다음으로 옴)

<thead>,<tbody>,<tfoot>: 표 구조 (제목, 본문, 요약)

<col>,<colgroup>: 열을 묶어 스타일 지정


// 이미지, 링크 //

<img src = “ “>: 이미지 (alt: 이미지 대체 텍스트) (width, height 속성)

<figure>, <figcaption>: 설명 글 붙이기

<a href = “ “>: 링크 생성 (targe_self: 그 곳에서 열림, target_blank: 새창, 새탭에서 열림)

ㄴ Anchor 제작: <태그 id = “앵커 이름”> 텍스트/이미지 </태그>

<a href = “#앵커 이름”> 텍스트/이미지 </a>

<map name=”맵이름”>, <area>, <img src=”이미지 파일” usemap=”#맵이름”>: 이미지 맵 지정

​

// 폼 태그, 폼 요소 //

<form>: 폼 만들기 (action 속성으로 서버 프로그램 지정) (autocomplete 속성: 자동 완성 기능)

<label>: 폼 요소에 레이블 지정 (폼 요소 앞뒤에 레이블 태그를 붙이는 방법, id 속성을 이용해 적용하는 방법) 

(라디오 버튼과 체크박스에서 id 속성을 이용해 레이블 태그를 사용하면 텍스트만 클릭해도 선택 가능)

<field>, <legend>: 폼 요소 그룹 묶기 (field: 외곽선 그리기, legend: 묶은 그룹의 제목)

<input>: 사용자 입력 태그 (id 속성 사용! Type 속성으로 다양하게 사용 가능) (autofocus: 입력 커서 표시, placeholder: 힌트 표시 (필드 클릭시 힌트 내용이 사라짐), readonly: 읽기 전용 필드, required: 필수 입력 필드, min: 최솟값, max: 최댓값, step: 숫자 간격 조절, size: 글자 사이즈 조절, minlength: 최소 입력 글자, maxlength: 최대 입력 글자, formmethod: 서버로 폼 전송하는 방식 지정, formnovalidate: 서버로 전송할 때 폼 데이터 유효성 여부 표시, formtarget: 폼 데이터를 서버에 전송후 서버 응답을 어디에 표시할지 타깃 지정, 

type=”hidden”: 히든 필드 (관리자가 알아야 하는 것) (name 속성으로 이름 지정, value 속성으로 서버로 전송)

type=”text”: 텍스트 필드 (한 줄짜리 텍스트) (name: 이름 지정, size: 화면에 보이는 글자 개수 지정, value: 텍스트 필드 부분에 표시될 내용, maxlength: 최대 문자 개수)

type=”password”: 비밀번호 입력란 (입력 내용이 ‘*’, ‘•’ 으로 표시됨)

type=”search”: 검색 상자

type=”url”: URL 입력란 (반드시 ‘http://’로 시작하는 사이트 주소만 입력해야 함)

type=”email”: 메일 주소 입력란 (메일 주소 형식에 맞는지 자동 체크, multiple: 두 개 이상의 값 입력)

type=”tel”: 전화번호 입력란

type=”number”: 숫자 입력 (스핀 박스 표시) (min: 최솟값, max: 최댓값, step: 숫자 간격, value: 필드에 표시할 초기값)

type=”range”: 슬라이드 막대로 숫자 지정 (min: 최솟값(기본: 0), max: 최댓값(기본: 100), step: 숫자 간격, value: 필드에 표시할 초기값)

type=”radio”: 라디오 버튼 (하나만 선택 가능) (name: 여러 개 있을 때 구분, value: 서버로 넘길 값(필수), checked: 기본으로 선택해 놓을 값)

type=”checkbox”: 체크박스 (여러 개 선택 가능) (name: 여러 개 있을 때 구분, value: 서버로 넘길 값(필수), checked: 기본으로 선택해 놓을 값)

type=”color”: 색상 선택 상자 

type=”date”: 연도, 월, 일 선택 (yyyy-mm-dd)

type=”month”: 연도, 월 선택 (yyyy-mm)

type=”week”: 연도, 주 선택

type=”time”: 시간 선택 (시, 분, 초, 분할 초) (min: 최솟값, max: 최댓값, step: 간격 조절, value: 화면에 표시할 초기값(00:00 ~ 23:59)

type=”datetime”: 국제 표준시(UTC)로 설정된 날짜와 시간 선택 (연, 월, 일, 시, 분, 초, 분할 초) (min: 최솟값, max: 최댓값, step: 간격 조절, value: 화면에 표시할 초기값(날짜 다음에 T를 쓰고 24시간제로 시간 지정)

type=”datetime-local”: 사용자 지역을 기준으로 날짜와 시간 선택 (연, 월, 일, 시, 분, 초, 분할 초) (min: 최솟값, max: 최댓값, step: 간격 조절, value: 화면에 표시할 초기값(날짜 다음에 T를 쓰고 24시간제로 시간 지정)

type=”submit”: 서버 전송 버튼 (value: 버튼에 표시될 내용, formaction: 실행할 프로그램 연결, formenctype: 서버로 폼 전송시 폼데이터 해석 방식 지정)

type=”reset”: 리셋 버튼 (value: 버튼에 표시될 내용)

type=”image”: submit 버튼 대신 사용할 이미지, formaction: 실행할 프로그램 연결, formenctype: 서버로 폼 전송시 폼데이터 해석 방식 지정, height: 이미지 높이 지정, width: 이미지 너비 지정) 

type=”button”: 버튼 (스크립트 함수 등을 연결해 사용) (value: 버튼에 표시될 내용)

type=”file”: 파일 첨부 버튼 (multiple: 두 개 이상의 값 입력)


<select>: 드롭다운 목록의 시작과 끝 (size: 화면에 표시될 드롭다운 메뉴의 항목 개수(크롬일 경우 +1로 계산), multiple: 컨트롤키를 누른 상태로 여러 항목 선택 가능)

<option>: 드롭다운 목록의 항목 (value: 옵션 선택시 서버로 넘겨질 값, selected: 기본 선택값)

<optgroup>: 드롭다운 목록에서 여러 항목들을 몇 가지 그룹으로 묶을 때 사용 (label 속성으로 그룹 제목 지정)

<datalist>: 위의 select 대신 사용시 데이터 목록(number, ranger, color 등) 중에서 값을 선택하게 할 수 있음 (value: 서버로 넘겨질 값, label: 브라우저에 표시할 레이블 값)

<textarea>: 한줄 이상의 문장 입력 (name: 텍스트 영역의 이름 지정, cols: 가로 너비(px), rows: 세로 길이(줄))

<button>: 버튼 태그 (type=”submit”: 폼을 서버로 전송, type=”reset”: 폼에 입력한 모든 내용 초기화, type=’button”: 버튼 형태)

<output>: 계산 결과

<progress>: 진행 상태 (value: 작업 진행 상태. 부동 소수점으로 표현 (0보다 크거나 같고, max 값보다 작아야됨 (max값이 없으면 1보다 작아야됨), max: 작업 완료 상태. 부동소수점으로 표현 (0보다 커야함))

<meter>: 값이 차지하는 크기 (min: 최솟값 (0), max: 최댓값 (1), value: 범위 내 차지하는 값, low: “이 정도면 낮다”라는 정도의 값, high: “이 정도면 높다”라는 정도의 값, optimum: “이 정도면 적당하다”라는 정도의 값)

​

// 시맨틱 태그 //

>> 이름만 보고도 문서 구조에서 어떤 역할을 하는지 알 수 있는 태그 (웹 접근성에서 매우 중요)

<header>: 머리말 (주로 페이지 맨 위쪽, 왼쪽에 삽입 / 내용: <form> 태그를 사용한 검색창, <nav> 태그를 사용한 사이트 메뉴 등)

<nav>: 내비게이션 링크 (footer에 있는 사이트 링크 모음 부분에서도 많이 사용 → 위치 영향 X)

<section>: 주제별 콘텐츠 영역 (<h1>~<h6> 태그를 이용해 섹션 제목을 나타냄)

<article>: 콘텐츠 내용 (보통 블로그 포스트, 웹사이트 내용, 사용자 등록 코멘트, 독립적 웹 콘텐츠 항목 등)

<aside>: 본문 이외의 내용 표시 (광고, 링크 모음 등 사이드바)

<iframe>: 외부 문서 삽입 (인라인 프레임) (width: 너비, height: 높이, name: 이름, src: 문서 주소, seamless: 테두리를 없애 본문의 일부처럼 보이게 만듬)

<footer>: 제작 정보, 저작권 정보 (사이트 제작자의 연락처 등)

<address>: 사이트 제작자 정보, 연락처 정보 (footer 태그 안에 사용되며, 피드백을 위한 연락처 정보를 넣는데 사용)

<div>: 주로 콘텐츠를 묶어 CSS를 적용할 때 사용


// 2. 멀티미디어 //

<audio>: 오디오 파일 삽입 (src: 미디어 파일 경로, autoplay: 자동 재생, controls: 컨트롤 막대 표시, loop: 반복 재생, muted: 소리X, preload: 재생 전 파일 다운로드)

<video>: 비디오 파일 삽입 (src: 미디어 파일 경로, controls: 컨트롤 막대 표시, width: 너비, height: 높이, preload: 재생 전 파일 다운로드, loop: 반복 재생, muted: 소리X, autoplay: 자동 재생, poster: 오류로 재생 불가시 비디오 대체 이미지)

<source>: 여러 미디어 파일 한꺼번에 지정 (ogv, webm 등 브라우저 버전별 지원 파일 지정)(src: 미디어 파일 경로, type: 미디어 파일 유형, codecs: 비디오 코덱 지정)

<track>: 비디오 자막 추가 (kind: 자막 종류 지정, src: 자막 파일 경로, srclang: 사용한 언어, label: 자막 파일이 여러 개일 경우, 자막 식별을 위한 제목, default: 자막 파일이 여러 개일 경우, 기본으로 사용할 자막)

​

// CSS 기초 //

- 스타일 형식 >> 선택자 { 스타일 속성: 속성 값; } /* 스타일 주석 */

- 내부 스타일 시트: <head> 태그 사이에 <style> 태그 안에 작성

- 외부 스타일 시트: <head> 태그 사이에 <link> 태그를 이용해 연결

- 인라인 스타일: 해당 태그에 style 속성 이용 (간단한 스타일일 때 사용)

- 전체 선택자: * {속성: 속성 값; …}

- 태그 선택자: 태그 {스타일}

- 클래스 선택자: .클래스명 {스타일}

- id 선택자: #id명 {스타일}

- 그룹 선택자: 이름1, 이름2 … {스타일}

- 캐스캐이딩 (Cascading)

1. 스타일 우선순위: 

- 중요도 (Importance): 

A. 사용자 스타일 시트 > 제작자 스타일 시트

B. 중요 스타일 시트 = 뒤에 ‘!important’를 붙인 스타일

C. 브라우저 스타일 시트: 브라우저 기본 지정 스타일

- 명시도 (Specificity):

A. 인라인 스타일

B. id 스타일

C. 클래스 스타일

D. 태그 스타일

- Source Order: 중요도와 명시도가 같다면 소스 순서 적용. (나중에 온 스타일이 최종 적용됨)


2. 스타일 상속

- 자식 요소에서 별도로 스타일을 지정하지 않으면 부모 요소에 있는 스타일 속성들이 자식 요소로 전달됨 (글꼴 등)

- 부모 요소의 배경 이미지, 배경 색 등은 상속되지 않으며, 기본 값인 ‘투명’으로 지정됨

​

​

// 텍스트 스타일 //

font-family: 글꼴 지정 (두 단어 이상으로 된 글꼴일 경우 따옴표 사용 ex. “맑은 고딕” / 지정한 글꼴이 없을 경우를 대비해 쉼표를 이용해 두 번째, 세 번째 글꼴 지정)

@font-face: 웹 폰트 적용 (font- family: 글꼴 이름, src: url(글꼴 파일 경로), format (파일 유형))

font-size: 글자 크기 조절 (절대 크기(xx-small, x-small, small, medium, large, x-large, xx-large), 상대 크기(larger, smaller), 크기(em, ex, px, pt로 직접 지정(주로 px 사용, 모바일은 em 사용)), 백분율(%))

font-weight: 글자 굵기 지정 (normal(기본값), bold, lighter, bolder, 100~900(400: normal, 700: bold))

font-variant: 작은 대문자 표시 (대문자를 소문자 크기에 맞춘 것) (normal(기본값), small-caps(작은 대문자 표시)

font-style: 글자 스타일 지정 (normal(기본값), italic(이탤릭체. 주로 사용), oblique(원래 글꼴을 기울어지게 표시한 이탤릭체)

font: 글꼴 속성 한꺼번에 묶어 표시 (위에 있는 속성 + font-*(font-로 시작하는 속성 한꺼번에 나열, 폰트 크기와 높이는 ‘/’로 연결해 함께 표현), caption(캡션에 어울리는 글꼴 스타일 표시, icon(아이콘에 어울리는 글꼴 스타일 표시), menu(드롭다운 메뉴에 어울리는 글꼴 스타일 표시), message-box(대화상자에 어울리는 글꼴 스타일 표시), small-caption(작은 캡션에 어울리는 글꼴 스타일 표시), status-bar(상태 표시줄에 어울리는 글꼴 스타일 표시)

color: 글자 색 지정 (16진수, rgb(rgba), hsl(hsla), 색상 이름)

text-decoration: 텍스트에 줄 표시 (none: 밑줄 표시 X, underline: 밑줄 표시, overline: 영역 위로 선 표시, line-through: 취소선 표시)

text-transform: 텍스트 대소문자 변환 (none: 변환 X, capitalize: 첫 번째 글자 대문자로 변환, uppercase: 모든 글자 대문자로 변환, lowercase: 모든 글자 소문자로 변환, full-width: 모든 문자 전각 문자(고정 너비의 두배 너비의 문자)로 변환)

text-shadow: 텍스트 그림자 효과 (가로 거리 (양수값: 글자 오른쪽, 음수값: 글자 왼쪽), 세로 거리 (양수값: 글자 위쪽, 음수값: 글자 아래쪽), 번짐 정도(양수값: 그림자 크게 표시, 음수값: 그림자 작게 표시, 기본값: 0), 색상)

white-space: 공백 처리 (normal (여러 개의 공백을 하나로 처리(기본값)), nowrap (여러 개의 공백을 하나로 처리, 영역 너비를 넘어가는 내용은 줄바꿈없이 계속 한줄로 표시), pre (여러 개의 공백을 그대로 표시, 영역 너비를 넘어가는 내용은 줄바꿈없이 계속 한줄로 표시), pre-line (여러 개의 공백을 하나로 처리, 영역 너비를 넘어가는 내용은 줄바꿔 표시), pre-wrap (여러 개의 공백을 그대로 표시, 영역 너비를 넘어가는 내용은 줄바꿔 표시)

letter-spacing: 낱 글자 사이 간격 조절 (글꼴 변경을 위해 em 단위 지정이 좋음)

word-spacing: 단어와 단어 사이 간격 조절 (글꼴 변경을 위해 em 단위 지정이 좋음)

direction: 글자 쓰기 방향 지정 (ltr(left to right 왼쪽에서 오른쪽으로), rtl(right to left 오른쪽에서 왼쪽으로))

text-align: 텍스트 정렬 (start(현재 텍스트 줄의 시작 위치에 맞추어 정렬), end(현재 텍스트 줄의 끝 위치에 맞추어 정렬), left(왼쪽에 맞추어 정렬), right(오른쪽에 맞추어 정렬), center(가운데에 맞추어 정렬), justify(양쪽에 맞추어 정렬), match-parent(부모 요소를 따라 문단 정렬)

text-justify: 정렬시 공백 조절 (auto (자동 지정), none (정렬 X), inter-word (단어 사이 공백 조절), distribute (인접 글자 사이의 공백을 똑같이 맞추어 정렬)

text-indent: 문단 첫 글자 들여 쓰기 (크기(음수값도 사용 가능), 백분율(부모 요소 기준 상대적 크기))

line-height: 줄 간격 조절 (normal, 숫자(배수), 크기, 백분율, inherit)

text-overflow: 넘치는 텍스트 표시 (overflow 속성 값이 hidden, scroll, auto이면서 white-space: nowrap일 때 처럼 텍스트가 넘칠 때 사용) (clip(넘치는 텍스트 자름), ellipsis(말 줄임표(…)로 표시)) 

list-style-type: 목록 불릿, 번호 스타일 지정 (disc: 채운 원, circle: 빈 원, square: 채운 사각형, none: 불릿 X, decimal: 1로 시작하는 십진수, decima-leading-zero: 앞에 0이 붙는 십진수, lower-roman: 소문자 로마 숫자, upper-roman: 대문자 로마 숫자, lower-alpha(lower-latin): 소문자 알파벳, upper-alpha(upper-latin): 대문자 알파벳, armenian: 아르메니아 숫자, georgian: 조지 왕조시대 숫자

list-style-image: 불릿을 원하는 이미지로 대체 (none, url())

list-style-position: 목록에 들여쓰기 효과 내기 (inside: 불릿, 숫자 안쪽으로 들여씀, outside: 기본값)

list-style: 목록 속성 한꺼번에 표시

​

// 배경 스타일 //

- 색상 표기법

1. 16진수 표기법: #RRGGBB 형식으로 각 자리에 빨간색, 초록색, 파란색의 양을 표시함.

사용할 수 있는 값: #000000(검은색) ~ #ffffff(흰색) (0 ~ 9 + a ~ f)

2. rgb (rgba) 표기법: rgb(red값, green값, blue값, alpha값)으로 차례대로 나타내며,

하나도 섞이지 않았을 때는 0, 가득섞였을 때는 255로 표시.

alpha는 불투명도 값을 나타낸 것 (1은 완전히 불투명, 0은 완전히 투명)

3. hsl (hsla) 표기법: hue (색상), saturation (채도), lightness (밝기)를 차례대로 나타냄.

색상: 0°와 360°에서 빨간색, 120°에서 초록색, 240°에서 파란색이 배치됨

채도: 0%면 회색 톤, 100%면 순색으로 표시.

밝기: 0%면 가장 어둡고 100%가 가장 밝음.

alpha는 rgba처럼 불투명도 값을 나타낸 것 (1은 완전히 불투명, 0은 완전히 투명)

4. 색상 이름 표기법: 색상 이름으로 표시 (기본 16가지 색상(aqua, black, blue, fuchsia, gray, green, lime, maroon, navy, olive, purple, red, silver, teal, white, yellow) + 200가지 색상)


- 배경 색 지정

background-color: 배경 색 지정

background- clip: 배경 적용 범위 조절 (border-box: 테두리까지 적용, padding-box: 패딩 범위까지 적용, content-box: 내용 부분에 적용)

background-image: 배경 이미지 넣기 (url(파일 경로))

background-repeat: 배경 이미지 반복 방법 지정 (배경 이미지의 크기가 배경을 채우려는 요소보다 작을 경우, 반복해 표시) (repeat: 가로와 세로 반복, repeat-x: 가로로 반복, repeat-y: 세로로 반복, no-repet: 반복 X)

background-size: 배경 이미지 크기 조절 (auto: 원래 배경 이미지 크기만큼 표시, contain: 배경 이미지가 다 들어오도록 이미지 확대/축소, cover: 요소 전체를 모두 덮도록 이미지 확대/축소, 크기값: 너비 값과 높이 값 지정, 백분율: 백분율 값 지정)

background-position: 배경 이미지 위치 조절 

- 키워드 표시법: 수평 위치: left, center, right / 수직 위치: top, bottom, center

- 백분율(%) 표시법: 0% 0%라면 요소의 왼쪽 모서리에 배경 이미지의 왼쪽 모서리를 맞춤

- 길이(px) 표시법: 픽셀로 지정하여 위치를 맞춤

background-origin: 배경 이미지 배치 기준 조절 (border-box: 테두리 기준, padding-box: 패딩 기준, content-box: 내용 부분)

background-attachment: 배경 이미지 고정 (scroll: 화면 스크롤과 함께 배경 이미지도 스크롤됨, fixed: 화면 스크롤이 되도 배경 이미지는 고정)

background: 배경 이미지 속성 하나로 묶어 표시

linear-gradient: 선형 그러데이션 (방향: to top(아래에서 위로), to left(오른쪽에서 왼쪽으로), to right(왼쪽에서 오른쪽으로), to bottom(위에서 아래로) / 각도: 맨 윗부분이 0deg, 시계방향으로 90deg, 180deg, 270deg / 색상 중지 점: 바뀌는 지점의 색상)

radial-gradient: 원형 그러데이션 (모양: circle(원형), ellipse(타원형) / 위치: 그러데이션 시작 원의 중심 지정 (at 키워드 사용) (키워드(left, center, right 중 하나, top, center, bottom 중 하나), 백분율) / 크기: closest-side (가장 가까운 모서리와 만남), closest-corner (가장 가까운 코너와 만남), farthest-side (가장 먼 모서리와 만남), farthest-corner (가장 먼 코너와 만남) / 색상 중지 점: 색상이 바뀌는 위치 지정)

repeating-linear-gradient: 선형 그러데이션 반복 

repeating-radial-gradient: 원형 그러데이션 반복


// 레이아웃 스타일 //

- 블록 레벨 (block-level) 요소: 혼자 한 줄을 차지하는 요소

ex) <p>, <h1>~<h6>, <ul>, <ol>, <div>, <blockquote>, <form>, <hr>, <table>, <fieldset>, <address>

- 인라인 레벨 (inline-level) 요소: 줄을 차지하지 않는 요소, 같은 줄에 섞여 표시됨

ex) <img>, <object>, <br>, <sub>, <sup>, <span>, <input>, <textarea>, <label>, <button>

- 박스 모델 (box model): 박스 형태의 콘텐츠 (콘첸츠 영역, 패딩, 테두리, 마진 등의 요소로 구성됨)

width, height 속성: 콘텐츠 영역 크기 (크기(px, em 등), 백분율, auto(자동으로 결정))

*실제 박스 모델의 전체 너비 = width 값 + 좌우 패딩 + 좌우 테두리

display 속성: 화면 배치 방법 결정 (세로 목록을 가로 내비게이션으로 바꿀 때, 한줄로 표시되는 이미지를 갤러리로 표시할 때 사용함) (block: 해당 요소를 블록 레벨로 지정, inline: 해당 요소를 인라인 레벨로 지정, inline-block: 블록 레벨 요소와 인라인 레벨 요소 두 가지 특성을 모두 가짐, none: pc에선 표시하지만 모바일에서 보이지 않도록 하고 싶을 때 사용 (공간조차 차지하지 않음), inherit: 상위 요소 상속, table: 블록 레벨의 표로 제작, inline-table: 인라인 레벨의 표로 제작(=<table>), table-row: 표의 행 제작(=<tr>), table-row-group: 표의 행 그룹 제작(=<tbody>), table-header-group: 표의 제목 영역 그룹 제작(= <thead>), table-footer-group: 표의 요약 영역 그룹 제작(=<tfoot>), table-column: 표의 열 제작(=<col>), table-column-group: 표의 열 그룹 제작(=<colgroup>), table-cell: 표에서 하나의 셀로 제작(=<td>, <th>), table-caption: 표의 캡션 제작(=<caption>), list-item: 목록 항목 표시를 위해 기본적인 블록 박스(불릿이 표시되는 부분)와 표시자 박스 제작(=<li>)

border-style 속성: 테두리 스타일 지정 (none: 테두리 X, hidden: 테두리 표시 X, dashed: 짧은 선 테두리 (직선 점선), dotted: 점선 테두리, double: 이중선(겹선), groove: 조각 같은 입체 테두리, inset: 조각 같은 테두리(border-collapse에 따라 다름), outset: 창에서 튀어나온 것 같은 테두리 (border-collapse에 따라 다름), ridge: 창에서 튀어나온 것 같은 테두리, solid: 실선 테두리

​

// CSS 포지셔닝 //

box-sizing: 박스 너비 기준 (content-box: width 속성 값을 콘텐츠 영역 너비 값으로 사용, border-box: width 속성 값을 박스 모델 전체 너비 값으로 사용)

float: 요소를 왼쪽이나 오른쪽으로 배치 (left: 문서 왼쪽으로 배치, right: 문서 오른쪽으로 배치, none: 배치X)

clear: float 속성 해제 (none: 해제 X, left: “float:left” 해제, right: “float:right” 해제, both: 왼쪽, 오른쪽 상관없이 해제)

position: 요소 배치 방법 지정 (static: 문서 흐름에 맞추어 배치, relative: 이전 요소와 자연스럽게 배치(위치 지정 가능), absolute: 원하는 위치 지정 가능, fixed: 지정한 위치에 고정(스크롤해도 고정됨, 요소가 잘릴 수 있음)

visibility: 요소를 보이게, 보이지 않게 하기 (visible: 화면에 요소 표시, hidden: 화면에 요소 감춤(크기는 유지되므로 배치에 영향), collapse: 표의 행(열, 행 그룹, 열 그룹)에서 지정하면 겹침(그 외의 영역에선 hidden처리))

z-index: 요소 쌓는 순서 (숫자로 지정, 무조건 맨 앞에 표시해야 한다면 1000같은 매우 큰 값 사용)

column-width: 단의 너비 고정하고 다단 구성 (크기: 단 너비 직접 지정, auto: 단의 개수에 따라 단의 너비 자동 계산)(화면이 커지면 단의 개수가 많아지고, 좁아지면 단의 개수가 줄어듬)

column-count: 단의 개수 고정하고 다단 구성 (숫자: 단 개수 직정 지정, auto: 단의 너비에 따라 단의 개수 자동 계산)(단의 개수는 항상 일정, 화면이 커지면 단의 너비도 커짐)

column-gap: 단과 단 사이 여백 지정 (크기: 여백을 숫자로 지정, normal: 자동 지정(W3C 권장 여백: 1em))

column-rule: 구분선 색상, 스타일, 너비 지정 (너비: 크기값, thin, medium, thick / 스타일: none, hidden, dotted, dashed, solid, double, groove, ridge, inset, outset / 섹상)

break-after: 다단 위치 지정 (”break-before:column”: 특정 요소 앞부분에서 단 나누기 / ”break-after:column” 특정 요소 뒤에서 단 나누기 / ”break-inside:column”: 특정 요소 안에서 단 나누기 / ”break-before:avoid-column” 특정 요소 앞부분에서 단 나누지 않게 하기 / ”break-after:avoid-column” 특정 요소 뒤에서 단 나누지 않게 하기 / ”break-inside:avoid-column”: 특정 요소 안에서 단 나누지 않게 하기

column-span: 여러 단을 하나로 합치기 (1: 기본값(합치지 않음), all: 전체 단을 하나로 합침)


// 표 스타일 //

caption-side: 표 제목 위치 정하기 (top: 캡션을 표 윗부분에 표시, bottom: 캡션을 표 아랫부분에 표시)

border: 표 테두리 스타일 결정 (주로 “table border=”1” 처럼 사용)

border-collapse: 테두리 통합, 분리 (collapse: 테두리 하나로 통합, separate: 테두리 분리)

border-spacing: 인접한 셀 테두리 사이 거리 지정 (”border-collapse:separate”로 셀들을 분리했을 때 사용) (px, em 등으로 크기 직접 지정)

empty-cells: 비어있는 셀 표시 여부 지정 (”border-collapse:separate”로 셀들을 분리했을 때 사용) (show: 빈 셀 표시, hide: 테두리없이 비워둠)

width, height 속성: 표와 셀의 너비, 높이 지정

table-layout: 콘첸츠에 맞게 셀 너비 지정 (fixed: 셀 너비 고정, auto: 셀 내용에 따라 너비가 달라짐)

text-align: 셀 안에서 수평 정렬 (left, right, center)

vertical-align: 셀 안에서 수직 정렬 (baseline, top, bottom, middle, sub, super, text-top, text-bottom, 길이값, 백분율값)

​

// 연결 선택자 //

하위 선택자 (=자손 선택자 / descendant selector): 모든 하위 요소에 스타일 적용

기본형: 상위요소 하위요소 {속성} / ex) section p {color:bue;}

자식 선택자 (child selector): 자식 요소에만 스타일 적용

기본형: 부모요소 > 자식요소 {속성} / ex) section > p {color:blue;}

인접 형제 선택자 (adjacent selector): 같은 형제 요소 중 첫 번째 동생 요소에만 스타일 적용

※ 같은 부모 요소를 가지는 요소: 형제 관계 / 먼저나오는 요소: 형 요소 / 나중에 나오는 요소: 동생 요소

기본형: 요소 1 + 요소 2 {속성} / ex) h1 + p {text-decoration: underline;}

형제 선택자 (sibling selectop): 모든 동생 요소에 스타일 적용

기본형: 요소 1 ~ 요소 2 {속성} / ex) h1 ~ p {text-decoration: underline;}


// 속성 선택자 //

[속성] 선택자: 지정한 속성에 스타일 적용

기본형: [속성] {속성} / ex) a[href] {background: yellow;}

[속성 = 값] 선택자: 속성과 속성 값이 일치하는 요소를 찾아 스타일 적용

기본형: [속성 = 값] {속성} / ex) a[target=”_blank”] {padding-right: 30px;}

[속성 ~= 값] 선택자: 여러 속성 값 중에 해당 값이 포함되어 있으면 스타일 적용

※ 한 단어로 일치해야하며, 하이픈으로 연결되어 있거나 일부만 일치할 때는 적용 X

기본형: [속성 ~= 값] {속성} / ex) [class ~= “button”] {border: 2px solid, black;}

[속성 |= 값] 선택자: 특정 값이 포함된 속성에 스타일 적용

※ 한 단어로 일치해야하며, 하이픈으로 연결한 단어도 스타일 적용

기본형: [속성 |= 값] {속성} / ex) a[title |= “us”] {padding: 5px 25px;}

[속성 ^= 값] 선택자: 지정한 문자로 시작하는 속성 값에 대해서만 스타일 적용

기본형: [속성 ^= 값] {속성} / ex) [title ^= “eng”] {padding: 5px 25px;}

[속성 $= 값] 선택자: 특정 값으로 끝나는 속성에 스타일 적용

기본형: [속성 $= 값] {속성} / ex) a[hreg $= “hwp”] {padding-right: 25px;}

[속성 *= 값] 선택자: 어느 위치든 해당 값이 포함되어 있으면 스타일 적용

기본형: [속성 *= 값] {속성} / ex) [href *= “w3”] {color: white;}


// 가상 클래스 (pseudo class) //

- 사용자 동작에 반응하는 가상 클래스

:link 선택자: 방문하지 않은 링크에 스타일 적용

:visited 선택자: 방문한 링크에 스타일 적용

:hover 선택자: 웹 요소에 마우스 커서를 올렸을 때 스타일 적용

:active 선택자: 웹 요소를 활성화했을 때 스타일 적용

:focus 선택자: 웹 요소에 포커스를 맞추었을 때 스타일 적용

- UI 요소 상태에 따른 가상 클래스

:enabled와 :disabled 선택자: 요소 사용할 수 있을 때와 없을 때 스타일 지정

ex) 게시판 입력시 enabled 상태, 읽기 상태일 때 disabled 상태

:checked 선택자: 라디오 박스, 체크 박스에서 해당 항목 선택시 스타일 적용

- 구조 가상 클래스 (특정 위치에 있는 요소를 찾아 스타일 지정)

:root 선택자: 문서 전체에 적용

:nth-child(n)와 :nth-last-child(n) 선택자: 지정할 항목이 몇 번째에 있는지를 따져 스타일 지정 (주로 메뉴항목)

:nth-child(n): 앞에서부터 n번째 자식 요소에 스타일 적용

:nth-last-child(n): 끝에서부터 n번째 자식 요소에 스타일 적용

an+b처럼 수식 사용 가능 ex) 2n+1

※해당 요소들이 모두 한 부모 요소를 갖고 있어야 함

:nth-of-type(n), :nth-last-of-type(n) 선택자: 태그에 따라 몇 번째에 있는 항목인지를 지정해 스타일 적용 :nth-of-type(n): 앞에서부터 세어 n번째 요소에 스타일 적용

:nth-last-of-type(n): 끝에서부터 세어 n번째 요소에 스타일 적용

:first-child, :last-child 선택자: 첫 번째, 마지막 요소에 스타일 적용

:first-child: 첫 번째 자식 요소를 선택해 스타일 적용

:last-child: 마지막 자식 요소에 스타일 적용

:first-of-type, :last-of-type 선택자: 형제 관계 요소의 위치에 따라 스타일 적용

:first-of-type: 첫 번째 요소에 스타일 적용

:last-of-type: 마지막 요소에 스타일 적용

:only-child, :only-of-type 선택자: 하나뿐인 자식 요소에 스타일 적용

:only-child: 부모 요소 안의 자식 요소가 유일하게 하나일 때 스타일 적용

:only-of-type: 해당 요소가 유일한 요소일 때 스타일 적용

- 그 외 가상 클래스

:target 선택자: 앵커 목적지에 스타일 적용

:not 선택자: 특정 요소가 아닐 때 스타일 적용 (괄호 안에 있는 요소 제외)

ex) p:not(#ex) {color:blue;} 

- 가상 요소 (내용 일부만 선택해 스타일 적용할 때 사용, 클래스 이름 앞에 콜론 두 개(::)를 붙여 표시

::first-line와 ::first-letter 요소: 첫 번째 줄, 첫 번째 글자에 스타일 적용

※::first-letter에서 첫 번째 글자는 반드시 첫 번째 줄에 있어야 함

::before, ::after 요소: 내용 앞뒤에 콘텐츠(텍스트, 이미지 등) 추가


// 변형 //

기본형: {transform: 변형함수;} / ex) .photo {transform: translate(50px, 100px);}

- 2차원 변형 함수

translate (tx, ty): 지정한 크기만큼 x축과 y축으로 이동

translateX (tx): 지정한 크기만큼 y축으로 이동

translateY (ty): 지정한 크기만큼 x축으로 이동

scale(sx, sy): 지정한 크기만큼 x축과 y축으로 확대/축소

scaleX(sx): 지정한 크기만큼 x축으로 확대/축소

scaleY(sy): 지정한 크기만큼 y축으로 확대/축소

rotate(각도): 지정한 각도만큼 회전

skew(ax, ay): 지정한 각도만큼 x축과 y축으로 왜곡

​

// 반응형 레이아웃 //

- 뷰포트: 스마트폰에서 실제 화면이 표시되는 영역

기본형: <meta name=”viewport” content=”<속성1=값>, <속성2=값2>, …”>

※속성: width, height, user-scalable, initial-scale, minimum-scale, maximum-scale

- 가변 그리드 레이아웃: 전체를 감싸는 요소의 너비를 기준으로 각 요소 너비 계산

※(요소의 너비 / 콘텐츠 전체를 감싸는 요소의 너비) * 100

- 가변 글꼴

1. em 단위: 글자 크기(em) = 글자 크기(px) / 16px

※1em = 16px

2. rem 단위: 처음부터 기본 크기를 지정하여 부모 요소의 크기에 따라 자식 요소의 글자 크기가 바뀌는 em 단위의 단점을 보완함.

- 가변 이미지

<img>태그의 srcset 속성, <picture>, <source> 태그 이용

- 가변 비디오

<video> 태그에서 max-width 속성을 100%로 지정


// 미디어 쿼리 //

기본형: @media [only | not] 미디어 유형 [and 조건] * [and 조건]

1. 연산자

- and: 조건 계속 추가

- ,(쉼표): 동일한 스타일 유형이 있다면 쉼표로 추가

- only: 미디어 쿼리 지원 브라우저에서만 조건 인식

- not: 지정하는 미디어 유형 제외 ex) not tv

2. 미디어 유형

- all: 모든 미디어 유형

- print: 인쇄 장치

- screen: 컴퓨터, 스마트폰 스크린

- tv: 음성, 영상 동시 출력 TV

- aural: 음성 함성 장치 (화면 소리 출력 장치)

- braille: 점자 표시 장치

- handheld: 패드처럼 손에 들고 다니는 장치

- projection: 프로젝터

- tty: 디스플레이 기능 제한 장치 (픽셀 사용 X)

- embossed: 점자 프린터

3. 조건

- 웹 문서의 가로 너비, 세로 높이: width, height, min-width, min-height, max-width, max-height

- 단말기의 가로 너비, 세로 높이: device-width, device-height, min-device-width, min-device-height, max- device-width, max-device-height

- 화면 회전: orientation: portrait(세로 방향), orientation: landscape(가로 방향)

- 화면 비율: aspect-ratio(화면 비율 너비값, 높이값), min-aspect-ratio(최소 화면 비율), max-aspect-ratio(최대 화면 비율), device-aspect-ratio(단말기 화면 비율 너비값, 높이값), min-device-aspect-ratio(단말기 최소 화면 비율), max-device-aspect-ratio(단말기 최대 화면 비율)

- 색상당 비트 수: color(비트 수), min-color(최소 비트 수), max-color(최대 비트 수)


4. 미디어 쿼리 적용

- <link> 태그 사용: <link rel=”stylesheet” media=”미디어쿼리조건” href:”css 파일 경로”>

-@import 구문 사용: @import url(css파일 경로) 미디어쿼리조건

- 웹문서에서 직접 정의: <style media=”미디어 쿼리 조건”> 스타일 규칙 </style>


// 플렉서블 박스 레이아웃 //

플렉서블 박스 레이아웃: 그리드 레이아웃을 기반으로 플렉스 박스를 원하는 위치에 배치하는 것.

- display: 플렉스 컨테이너 지정 (flex: 박스 레벨 요소로 정의 / inline-flex: 인라인 레벨 요소로 정의)

- flex-direction: 플렉스 방향 지정 (row: 주축을 가로로, 교차축을 세로로 지정, 플렉스 항목은 왼쪽에서 오른쪽으로 배치 / row-inverse: 주축을 가로로, 교차축을 세로로 지정, 플렉스 항목은 오른쪽에서 왼쪽으로 배치 / column: 주축을 세로로, 교차축을 가로로 지정, 플렉스 항목은 위쪽에서 아래쪽으로 배치 / column-inverse: 주축을 세로로, 교차축을 가로로 지정, 플렉스 항목은 아래쪽에서 위쪽으로 배치)

- flex-wrap: 플렉스 항목 줄 배치 (no-wrap: 한 줄에 표시 / wrap: 여러 줄에 표시 / wrap-reverse: 여러 줄에 표시, 기존 방향과 반대로 배치)

- flex-flow: 플렉스 방향과 줄 배치 한꺼번에 지정 (flex-flow: <플렉스 방향> <플렉스 줄 배치>)

- order: 항목 배치 순서 바꾸기 (0: 소스 순서대로 배치 / 숫자: 그 순서에 따라 배치)

- flex: 항목 크기 조절 (flex-grow: 너비를 얼마나 늘일지 숫자로 지정 / flex-shrink: 너비를 얼마나 줄일지 숫자로 지정 / flex-basis: 기본 크기 지정 / initial: 컨테이너 공간이 부족할 경우, 최소 크기까지 줄임 / auto)

- justify-content: 주축 기준 배치 방법 지정 (flex-start: 주축의 시작점 기준 / flex-end: 주축의 끝점 기준 / center: 주축의 중앙 기준 / space-between: 양쪽 끝 항목을 시작점과 끝점에 배치하고 나머지는 같은 간격으로 배치 / space-around: 모두 같은 간격으로 배치)

- align-items / align-self: 교차축 기준 배치 방법 지정 (stretch: 항목을 확장해 교차축을 꽉 채움 / flex-start: 교차축의 시작점 기준 / flex-end: 교차축의 끝점 기준 / center: 교차축의 중앙 기준 / baseline: 시작점과 글자 기준선이 가장 먼 플렉스 항목을 시작점에 배치)

- align-ccontent: 여러 줄일 때 배치 방법 지정 (flex-start: 주축의 시작점 기준 / flex-end: 주축의 끝점 기준 / center: 주축의 중앙 기준 / space-between: 양쪽 끝 항목을 시작점과 끝점에 배치하고 나머지는 같은 간격으로 배치 / space-around: 모두 같은 간격으로 배치)