<span style="color:#FF3232">

# **Markdown**

</span>

<span style="color:#FF5050">

## 0. Contents

</span>

- [1. Markdown Starting](#1-markdown-starting)
- [2. Markdown Basic Syntax](#2-markdown-basic-syntax)
- [3. Markdown Extended Syntax](#3-markdown-extended-syntax)
- [4. Markdown Hacks](#4-markdown-hacks)
- [5. Markdown Tools](#5-markdown-tools)
- [6. Markdown Books](#6-markdown-books)

<br>

---

<span style="color:#FF5050">

## 1. Markdown Starting

</span>

HTML Tag를 사용한 부분이 많이 있으나 GitHub Markdown에서는 적용이 안된 부분이 있습니다. 참고하여 보실 분들은 File을 다운받아 VSC에서 보시면 보다 편하게 보실 수 있습니다.

<br>

---

<span style="color:#FF5050">

## 2. Markdown Basic Syntax

</span>

<span style="color:#FF8282">

### 2.1 Overview

</span>

- 거의 모든 Markdown을 지원하는 Application에서는 기본 Markdown 문법을 제공
- Markdown Process 간에는 약간의 차이와 불일치 존재
- Markdown Syntax는 가능한 한 Inline으로 표시

<br>

---

<span style="color:#FF8282">

### 2.2 Heading

</span>

- 제목을 만들기 위해서는 # 기호를 단어 또는 문장 앞에 사용
- \# 기호의 개수가 많아질수록 크기가 작은 제목을 표현
- 대체 문법으로는 제목으로 사용할 텍스트 아래 == 또는 -- 추가
  - = 기호와 - 기호는 1개 이상 작성시 문법 적용
  - = 기호는 # 기호 1개와 동일 / - 기호는 # 기호 2개와 동일

<br>

<span style="color:#FFB4B4">

#### 2.2.1 Heading Syntax Cautions

</span>

- \# 기호와 제목 사이의 공백이 없을 경우 문법 적용 X
- 호환성을 위해 항상 # 기호와 제목 이름 사이에 공백이 필요
- 호환성을 위해 제목 앞 뒤에 빈 줄 추가

<br>

<span style="color:#FFB4B4">

#### 2.2.2 Heading Syntax

</span>

> \# TEST  
> \## TEST  
> \### TEST  
> \#### TEST  
> \##### TEST  
> \###### TEST  

<br>

<span style="color:#FFB4B4">

#### 2.2.3 Heading Alternate Syntax

</span>

> \# TEST  
> \=====  
> \# TEST  
> \-----

<br>

<span style="color:#FFB4B4">

#### 2.2.4 Heading Syntax Example

</span>

> Heading Syntax X  
> Test

> Heading Syntax O  
>
> # TEST
> 
> ## TEST
> 
> ### TEST
> 
> #### TEST
> 
> ##### TEST
> 
> ###### TEST

<div style="line-height:60%;">
  <br>
</div>

> Heading Alternate Syntax O  
> 
> TEST
> =
> 
> TEST
> -

<br>

---

<span style="color:#FF8282">

### 2.3 Paragraphs

</span>

- 단락 사이에 빈 줄을 사용하여 단락 구분

<br>

<span style="color:#FFB4B4">

#### 2.3.1 Paragraphs Syntax Cautions

</span>

- Line Breaks [ 줄바꿈 ]과 굉장히 굉장히 유사함
- 줄바꿈과 크게 다른 것이 없어보이지만 줄바꿈과는 줄 공백의 높이가 다름

<br>

<span style="color:#FFB4B4">

#### 2.3.2 Paragraphs Syntax

</span>

> TEST
> 
> TEST

<br>

<span style="color:#FFB4B4">

#### 2.3.3 Paragraphs Syntax Example

</span>

> Paragraphs Syntax X
> <br>
> TEST
> TEST

> Paragraphs Syntax O
> <br>
> TEST
> 
> TEST

> Line Breaks Syntax O
> <br>
> TEST
> <br><br>
> TEST

<br>

---

<span style="color:#FF8282">

### 2.4 Line Breaks

</span>

- 줄바꿈 또는 새로운 줄을 만들기 위해서는 문장의 끝 부분에 후행 공백 [ 두 개 이상의 Space 공백 ] 사용

<br>

<span style="color:#FFB4B4">

#### 2.4.1 Line Breaks Syntax Cautions

</span>

- 거의 모든 Markdown Application에서 후행 공백을 사용할 수 있지만 편집기에서 보기 어려움
- 대부분의 경우 사용시 후행 공백을 사용하여 작성하나 후행 공백 이외의 다른 것을 사용가능
- 호환성을 위해 후행 공백 또는 \<br> HTML Tag 사용
  - Markdown Application에서 HTML을 지원하는 경우 \<br> HTML Tag 사용 가능
  - \<br>은 줄바꿈을 표현
- 문장의 끝 부분에 백슬래시 [ \\ ]의 사용은 모든 Markdown Application에서 지원하는 것이 아니므로 사용 자제

<br>

<span style="color:#FFB4B4">

#### 2.4.2 Line Breaks Syntax

</span>

> TEST (Two Spaces)  
> TEST

> TEST  
> \<br>  
> TEST
 
<br>

<span style="color:#FFB4B4">

#### 2.4.3 Line Breaks Syntax Example

</span>

> Line Breaks Syntax X  
> TEST
> TEST

> Line Breaks Syntax O  
> TEST  
> TEST

> \<br> HTML Tag Line Breaks Syntax O  
> TEST
> <br>
> TEST

<br>

---

<span style="color:#FF8282">

### 2.5 Emphasis

</span>

- 텍스트를 Bold 또는 Italic으로 만들어 강조 표현

<br>

<span style="color:#FFB4B4">

#### 2.5.1 Emphasis Bold

</span>

- 단어 또는 문장 앞 뒤에 2개의 * 기호 또는 _ 기호를 추가하여 Bold 표현
- 문장 중간의 단어를 강조하기 위해 문장 중간의 단어 앞 뒤에 공백없이 2개의 * 기호 추가시 Bold 표현

<br>

<span style="color:#FFD2D2">

#### 2.5.1.1 Emphasis Bold Syntax Cautions

</span>

- 문장 중간의 단어에 Bold 표현을 하기 위해 단어 앞 뒤에 2개의 _ 기호를 사용할 경우 문법 적용 X

<br>

<span style="color:#FFD2D2">

#### 2.5.1.2 Emphasis Bold Syntax

</span>

> \*\*TEST\*\*  
> \_\_TEST\_\_  
> T\*\*ES\*\*T

<br>

<span style="color:#FFD2D2">

#### 2.5.1.3 Emphasis Bold Syntax Example

</span>

> Bold Syntax X  
> TEST

> Bold Syntax O  
> **TEST**  
> __TEST__  
> T**ES**T

<br>

<span style="color:#FFB4B4">

#### 2.5.2 Emphasis Italic

</span>

- 단어 또는 문장 앞 뒤에 1개의 * 기호 또는 _기호를 추가하여 Italic 표현
- 문장 중간의 단어를 강조하기 위해 문장 중간의 단어 앞 뒤에 공백없이 1개의 * 기호 추가시 Italic 표현

<br>

<span style="color:#FFD2D2">

#### 2.5.2.1 Emphasis Italic Syntax Cautions

</span>

- 문장 중간의 단어에 Italic 표현을 하기 위해 단어 앞 뒤에 1개의 _ 기호를 사용할 경우 문법 적용 X

<br>

<span style="color:#FFD2D2">

#### 2.5.2.2 Emphasis Italic Syntax

</span>

> \*TEST\*  
> \_TEST\_  
> T\*ES\*T

<br>

<span style="color:#FFD2D2">

#### 2.5.2.3 Emphasis Italic Syntax Example

</span>

> Italic Syntax X  
> TEST

> Italic Syntax O  
> *TEST*  
> _TEST_  
> T*ES*T

<br>

<span style="color:#FFB4B4">

#### 2.5.3 Emphasis Bold & Italic

</span>

- 단어 또는 문장 앞 뒤에 3개의 * 기호 또는 _기호를 추가하여 Bold 와 Italic을 동시에 표현
- 문장 중간의 단어를 강조하기 위해 문장 중간의 단어 앞 뒤에 공백없이 3개의 * 기호 추가시 Bold 와 Italic을 동시에 표현

<br>

<span style="color:#FFD2D2">

#### 2.5.3.1 Emphasis Bold & Italic Syntax Cautions

</span>

- 문장 중간의 단어에 Bold와 Italic을 표현하기 위해 단어 앞 뒤에 3개의 _ 기호를 사용할 경우 문법 적용 X

<br>

<span style="color:#FFD2D2">

#### 2.5.3.2 Emphasis Bold & Italic Syntax

</span>

> \*\*\*TEST\*\*\*  
> \_\_\_TEST\_\_\_  
> T\*\*\*ES\*\*\*T

<br>

<span style="color:#FFD2D2">

#### 2.5.3.3 Emphasis Bold & Italic Syntax Example

</span>

> Bold & Italic Syntax X  
> TEST

> Bold & Italic Syntax O  
> ***TEST***  
> ___TEST___  
> T***ES***T

<br>

---

<span style="color:#FF8282">

### 2.6 Blockquotes

</span>

- 인용구를 만들 단어 또는 문장 앞에 > 기호를 추가하여 표현
- \> 기호를 연달아 사용하여 여러줄의 인용구 표현
- 인용구를 중첩하여 사용하기 위해 \> 기호 2개를 단어 또는 문장 앞에 추가
- 인용구 내에 다른 Markdown Syntax 사용 가능
  - 모든 문법이 적용되는 것은 아니므로 Test 필요

<br>

<span style="color:#FFB4B4">

#### 2.6.1 Blockquotes Syntax Cautions

</span>

- 호환성을 위해 인용구 앞 뒤에 빈 줄 추가

<br>

<span style="color:#FFB4B4">

#### 2.6.2 Blockquotes Syntax

</span>

> \> TEST  
> \> TEST  
> \>> TEST  
> \> \- TEST

<br>

<span style="color:#FFB4B4">

#### 2.6.3 Blockquotes Syntax Example

</span>

> Blockquotes Syntax X  
> TEST

> Basic Blockquotes Syntax O  
> > TEST

> Blockquotes Syntax with Multiple Paragraphs O  
> > TEST  
> > TEST

> Nested Blockquotes Syntax O  
> > TEST  
> >> TEST

> Blockquotes Syntax With Other Syntax O  
> > TEST
> > - T***ES***T

<br>

---

<span style="color:#FF8282">

### 2.7 Lists

</span>

- 항목들을 정렬된 List와 정렬되지 않은 List로 구성

<br>

<span style="color:#FFB4B4">

### 2.7.1 Ordered List

</span>

- 숫자 뒤에 . 기호가 있는 줄을 추가하여 순서가 지정된 List 표현
- 번호는 번호순일 필요는 없으나 시작 숫자는 반드시 1부터 시작
- 중첩된 List를 만들기 위해서는 들여쓰기 2번 한 후 숫자 뒤에 . 기호가 있는 줄 추가
  - Ordered List 내 Unordered List를 중첩하여 사용 가능

<br>

<span style="color:#FFD2D2">

### 2.7.1.1 Ordered List Cautions

</span>

- 일부 Markdown Application에서 ) 기호를 . 기호 대신으로 사용할 수 있으나 호환성을 위해 . 기호만 사용

<br>

<span style="color:#FFD2D2">

### 2.7.1.2 Ordered List Syntax

</span>

> 1\. TEST  
> 2\. TEST  
> 3\. TEST  
> 4\. TEST

> 1\. TEST  
> 1\. TEST  
> 1\. TEST  
> 1\. TEST

> 1\. TEST  
> 8\. TEST  
> 23\. TEST  
> 15\. TEST

> 1\. TEST  
> 2\. TEST  
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1\. TEST  
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2\. TEST  
> 3\. TEST  
> 4\. TEST

> 1\. TEST  
> 2\. TEST  
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TEST  
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TEST  
> 3\. TEST  
> 4\. TEST

<br>

<span style="color:#FFD2D2">

### 2.7.1.3 Ordered List Syntax Example

</span>

> Ordered List Syntax X  
> TEST

> Ordered List Syntax O
> 1. TEST  
> 2. TEST  
> 3. TEST  
> 4. TEST

> Only One Number Ordered List Syntax O
> 1. TEST  
> 1. TEST  
> 1. TEST  
> 1. TEST

> Random Number Ordered List Syntax O
> 1. TEST  
> 8. TEST  
> 23. TEST  
> 15. TEST

> Nested Ordered List Syntax O
> 1. TEST  
> 2. TEST  
>     1. TEST  
>     2. TEST  
> 3. TEST  
> 4. TEST

> Use Unordered Syntax in the Ordered List Syntax O
> 1. TEST  
> 2. TEST  
>     - TEST  
>     - TEST  
> 3. TEST  
> 4. TEST

<br>

<span style="color:#FFB4B4">

### 2.7.2 Unordered List

</span>

- \- / \* / \+ 기호가 있는 줄을 추가하여 순서가 지정되지 않은 List 표현
- 줄 내용중 숫자와 . 기호를 포함한 내용이 있는 경우 . 기호 앞에 \\ [ Escape ]를 사용하여 정렬 List 표현 제한
- 중첩된 List를 만들기 위해서는 들여쓰기 한 후 중첩전에 사용한 \- / \* / \+ 기호가 있는 줄 추가
  - Unordered List 내 Ordered List를 중첩하여 사용 가능

<br>

<span style="color:#FFD2D2">

### 2.7.2.1 Unordered List Cautions

</span>

- 호환성을 위해 연속된 List 내에서 \- / \* / \+ 기호를 혼합하지 않고 1가지 기호만 이어서 사용

<br>

<span style="color:#FFD2D2">

### 2.7.2.2 Unordered List Syntax

</span>

> \- TEST  
> \- TEST  
> \- TEST  
> \- TEST

> \* TEST  
> \* TEST  
> \* TEST  
> \* TEST

> \+ TEST  
> \+ TEST  
> \+ TEST  
> \+ TEST

> \- TEST  
> \- TEST  
> &nbsp;&nbsp;&nbsp;&nbsp;\+ TEST  
> &nbsp;&nbsp;&nbsp;&nbsp;\+ TEST  
> \- TEST  
> \- TEST

> \- TEST  
> \- TEST  
> &nbsp;&nbsp;&nbsp;&nbsp;1\. TEST  
> &nbsp;&nbsp;&nbsp;&nbsp;1\. TEST  
> \- TEST  
> \- TEST

<br>

<span style="color:#FFD2D2">

### 2.7.2.3 Unordered List Syntax Example

</span>

> Unordered List Syntax X  
> TEST

> \- Symbol Unordered List Syntax O
> - TEST  
> - TEST  
> - TEST  
> - TEST

> \* Symbol Unordered List Syntax O
> * TEST  
> * TEST  
> * TEST  
> * TEST

> \+ Symbol Unordered List Syntax O
> + TEST  
> + TEST  
> + TEST  
> + TEST

> Nested Unordered List Syntax O
> - TEST  
> - TEST  
>   + TEST  
>   + TEST  
> - TEST  
> - TEST

> Use Ordered Syntax in the Unordered List Syntax O
> - TEST  
> - TEST  
>     1. TEST  
>     2. TEST  
> - TEST  
> - TEST

<br>

<span style="color:#FFB4B4">

### 2.7.3 Use Another Syntax in the List

</span>

- List의 연속성을 유지하면서 다른 Syntax를 추가하려면 Space 공백 4개 또는 Tab 1개를 단어 또는 문장 앞에 추가
- Code Blocks은 List 내에서 Space 공백 8개 또는 Tab 2개를 단어 또는 문장 앞에 추가

<br>

<span style="color:#FFD2D2">

### 2.7.3.1 Use Another Syntax in the List Cautions

</span>

- List 내 다른 Syntax 사용시 사용하는 Syntax의 앞 뒤로 빈 줄을 추가
- 정렬 / 정렬되지 않은 List와 줄간격의 차이가 발생

<br>

<span style="color:#FFD2D2">

### 2.7.3.2 Use Another Syntax in the List Syntax

</span>
  
> 1\. TEST  
> 2\. TEST  
> <br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TEST  
> <br>
> 3\. TEST

> \- TEST  
> \- TEST  
> <br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\> TEST  
> <br>
> \- TEST

> \* TEST  
> \* TEST  
> <br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; TEST  
> <br>
> \* TEST

> \- TEST  
> \- TEST  
> <br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;>\<img src="https://mblogthumb-phinf.pstatic.net/MjAxOTEyMTdfMTE4/MDAxNTc2NTkzMzEzMjQ4.tda-l5AtH-amqiFmAtZzcWvN2xwMIs6MVHp1lLpLxMcg.VJL2bWBxvxLfxLml4usBhz1ixgxBcui2EEumAr6LPV4g.JPEG.prettysyjudy/IMG_7256.JPG?type=w800" width="200" height="200"/> 
> <br>
> \- TEST  
> <br>
> Image Source - https://m.blog.naver.com/prettysyjudy/221740818850 [빛날빈]

<br>

<span style="color:#FFD2D2">

### 2.7.3.3 Use Another Syntax in the List Syntax Example

</span>

> Use Another Syntax in the List Syntax X  
> TEST

> Use Paragraphs Syntax in the List Syntax O  
> 1. TEST  
> 2. TEST  
> 
>     TEST  
>
> 3. TEST

> Use Blockquotes Syntax in the List Syntax O 
> - TEST  
> - TEST  
> 
>   > TEST  
>
> - TEST

> Use Code Blocks Syntax in the List Syntax O
> * TEST  
> * TEST  
> 
>         TEST  
>
> * TEST

> Use Images Syntax in the List Syntax O
> - TEST  
> - TEST  
> 
>     <img src="https://mblogthumb-phinf.pstatic.net/MjAxOTEyMTdfMTE4/MDAxNTc2NTkzMzEzMjQ4.tda-l5AtH-amqiFmAtZzcWvN2xwMIs6MVHp1lLpLxMcg.VJL2bWBxvxLfxLml4usBhz1ixgxBcui2EEumAr6LPV4g.JPEG.prettysyjudy/IMG_7256.JPG?type=w800" width="200" height="200"/>
> 
> - TEST  
> <br>
> Image Source - https://m.blog.naver.com/prettysyjudy/221740818850 [빛날빈]

<br>

---

<span style="color:#FF8282">

### 2.8 Code

</span>

- 텍스트를 코드로 변환하여 표현 가능

<br>

<span style="color:#FFB4B4">

### 2.8.1 Backticks

</span>

- ` [ 백틱 ]기호를 사용하여 단어 또는 문장을 코드로 표현 가능

<br>

<span style="color:#FFD2D2">

### 2.8.1.1 Backticks Syntax

</span>

> \`TEST\`  
> T\`ES\`T

<br>

<span style="color:#FFD2D2">

### 2.8.1.2 Backticks Syntax Example

</span>

> Backticks Syntax X  
> TEST

> Backticks Syntax O  
> `TEST`  
> T`ES`T

<br>

<span style="color:#FFB4B4">

### 2.8.2 Escaping Backticks

</span>

- 코드로 표현하려는 단어 또는 문장에 1개 이상의 \` 기호가 포함된 경우 단어 또는 문장 전체를 \` 기호 2개로 묶어 표현 가능

<br>

<span style="color:#FFD2D2">

### 2.8.2.1 Escaping Backticks Syntax Cautions

</span>

- 코드로 표현하려는 단어 또는 문장의 끝 부분에 \` 기호가 있을 경우 \` 기호 2개와 표현하려는 \` 기호 사이에 공백 필요

<br>

<span style="color:#FFD2D2">

### 2.8.2.2 Escaping Backticks Syntax

</span>

> \`\` \`TEST\` \`\`  
> \`\`T\`ES\`T\`\`

<br>

<span style="color:#FFD2D2">

### 2.8.2.3 Escaping Backticks Syntax Example

</span>

> Escaping Backticks Syntax X  
> TEST

> Escaping Backticks Syntax O  
> `` `TEST` ``  
> ``T`ES`T``

<br>

<span style="color:#FFB4B4">

### 2.8.3 Code Blocks

</span>

- Space 공백 4개 또는 Tab 1개를 Code Block으로 표현하고 싶은 모든 줄 앞에 추가

<br>

<span style="color:#FFD2D2">

### 2.8.3.1 Code Blocks Syntax Cautions

</span>

- 호환성을 위해 Code Block 앞 뒤에 빈 줄 추가

<br>

<span style="color:#FFD2D2">

### 2.8.3.2 Code Blocks Syntax

</span>

> TEST  
> <br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TEST  
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TEST  
> <br>
> TEST

<br>

<span style="color:#FFD2D2">

### 2.8.3.3 Code Blocks Syntax Example

</span>

> Code Blocks Syntax X  
> TEST

> Code Blocks Syntax O  
> TEST  
>
>     TEST    
>     TEST  
>
> TEST

<br>

---

<span style="color:#FF8282">

### 2.8 Horizontal Rules

</span>

- 3개 이상의 \* 기호 또는 \- 기호 또는 \_ 기호를 한 줄에 단독으로 사용하여 수평선 표현 가능

<br>

<span style="color:#FFB4B4">

### 2.8.1 Horizontal Rules Syntax Cautions

</span>

- 호환성을 위해 수평선 앞 뒤에 빈 줄 추가

<br>

<span style="color:#FFB4B4">

### 2.8.2 Horizontal Rules Syntax

</span>

> \*\*\*  
> <br>
> \-\-\-  
> <br>
> \_\_\_

<br>

<span style="color:#FFB4B4">

### 2.8.3 Horizontal Rules Syntax Example

</span>

> Horizontal Rules Syntax X  
> <br>

> Horizontal Rules Syntax O
>
> ***
>
> <br>
>
> ---
>
> <br>
>
> ___

<br>































## 3. Markdown Extended Syntax

## 4. Markdown Hacks

## 5. Markdown Tools

## 6. Markdown Books
