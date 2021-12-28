# 정규표현식 (regxp)
정규표현식 regularxEpression
## 역할

- 문자 검색
- 문자 대체
- 문자 추출

## 테스트사이트

https://regexr.com/

## 정규식생성


```javascript


// 생성자 
new RegExp("표현","옵션")

new RegExp("[a-z]","gi")

// 리터럴

/[a-z]/gi

````

````javascript

const str= `

010-36250-4630
dkfsdfsd@naver.com the
The rest day
aabbccssaaThe
`
````

## 메소드

메소드 | 문법 | 설명

--|--|--

test | 정규식.test(문자열) | 일치여부 (Boolean) 반환

match | 문자열.match(정규식) | 일치하는 문자의 배열(Array) 반환
replace | 문자열.replace(정규식, 대체문자) | 일치내용에 대체문자대체  


## 플래그 (옵션)

g = 글로벌 (모든문자 일치)
i = 이그노어 대소문자 (대소문자 상관없이 일치)
m = 여러줄 일치

## 패턴 

/^ab/ 줄 시작부분의 ab를 일치  
/ab$/ 줄 끝부분의 ab를 일치

a|b a또는b가 일치
ab? b가없거나 b와일치

{3} 3개일치
{3,} 3개이상 연속일치
{3,5} 3개이상 5개이하 (3,4,5) 일치
[abc] a또는b또는c
[a-z] a부터z사이의 모든 영어소문자
[A-Z] A부터Z사이의 모든ㅇ영어 대문자
[0-9] 0부터 9까지 숫자
[가-힣] 모든 한글 일치

\w | 63개 문자 (대소영문52개 + 숫자10개 + _)
\b | 63개 문자에 일치하지않는
문자경계(특수문자 등)
\d | 모든숫자 (Digit)
\s | 모든공백 (Space)

(?=) | 앞쪽일치
(?<=) | 뒤쪽일치