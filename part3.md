> ### 요소 5 : Lists

순서 없는 목록을 순서 목록에 중첩하거나 그 반대로 중첩할 수 있다.

      1. First item
      2. Second item
      3. Third item
          - Indented item
          - Indented item
      4. Fourth item

### The rendered output looks like this : 

1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item

<br>

## 7. Code (코드)

backticks(`)을 이용하여 코드를 나타낼 수 있다.

| Markdown | HTML | Rendered Output |
| --- | --- | ---- |
| At the command prompt, type \`nano\`. | At the command prompt, type \<code\>nano\</code\> | At the command prompt, type `nano`. |

<br>

## 8. Escaping Backticks

코드로 나타낼 단어 또는 구문에 하나 이상의 `가 포함되어 있는 경우, 단어 또는 구문을 이중 backticks(``)로 묶으면 이스케이프 할 수 있다.

| Markdown | HTML | Rendered Output |
| --- | --- | --- |
| \`\`Use \`code\` in your Markdown file.\`\` | \<code\>Use 'code' in your Markdown file.\</code\> | <code>Use 'code' in your Markdown file.</code> |

<br>

## 9. Code Blocks

코드 블록을 만들려면 블록의 모든 줄을 적어도 네 개의 공백 또는 한 개의 탭으로 들여쓴다.

    <html>
      <head>
      </head>
    </html>

<br>

## 10. Horizontal Rules (수평 규칙)

Horizontal rule을 만들려면 한 줄에 세 개 이상의 별표(***), 대시(---) 또는 밑줄(___)을 사용한다.

    ***
    ---
    ___

### The rendered output looks like this:

---

<br>

## Don't do this!

호환성을 위해 수평 규칙 앞뒤에 빈 줄을 놓아야 한다.  
그렇지 않으면 1.2가 적용될 확률 높다.

<br>

## 11.1 Links (링크)

링크를 만들려면 링크 텍스트를 대괄호로 묶은 다음 바로 다음에 URL을 괄호에 넣으면 된다.

    My favorite search engine is [youtube](https://www.youtube.com/).

### The rendered output looks like this:

My favorite search engine is [youtube](https://www.youtube.com/).

<br>

## 11.2 Adding Titles (제목 추가)

선택적으로 링크 제목을 추가할 수 있다. 사용자가 링크를 가리킬 때 툴팁으로 표시된다. 제목을 추가하려면 URL 뒤에 (")로 묶어야 한다.

    My favorite search engine is [youtube](https://www.youtube.com/ "I can't live without this!").

### The rendered output looks like this:

My favorite search engine is [youtube](https://www.youtube.com/ "I can't live without this!").

<br>

## 11.3 URLs and Email Addresses

URL 또는 전자 메일 주소를 빠르게 링크로 변환하려면 해당  주소를 꺽쇠 괄호로 묶어야 한다.

    <https://www.markdownguide.org>  
    <fake@example.com>

### The rendered output looks like this:

<https://www.markdownguide.org>  
<fake@example.com>

<br>

## 11.4 Formattion Links (링크 형식 지정)

링크를 강조하려면 괄호의 앞뒤에 별표를 추가한다.

링크를 코드로 나타내려면 괄호 안에 백틱을 추가한다.

    1. bold로 강조
    I  love supporting the **[EFF](https://eff.org)**. 

    2. italic으로 강조
    This is the *[Markdown Guide](https://www.markdownguide.org)*.

    3. 링크를 코드로 나타내기
    See the section on [`code`](#code)

### The rendered output looks like this:

I  love supporting the **[EFF](https://eff.org)**.
 
This is the *[Markdown Guide](https://www.markdownguide.org)*.

See the section on [`code`](#code)

<br>

## 11.5 Reference-style Links (참조 링크)

참조 링크는 URL을 Markdown에서 쉽게 표시하고 읽을 수 있도록 하는 특수한 종류의 링크이다. 참조 링크는 텍스트와 인라인으로 유지하는 부분과 텍스트를 읽기 쉽도록 파일의 다른 곳에 저장하는 부분의 두 부분으로 구성된다.

<br>

## 11.5.1 Formatting the First Part of the Link

참조 링크의 첫 번째 부분은 두 개의 대괄호 세트로 포맷된다. 첫 번째 대괄호 집합은 링크된 것으로 표시되는 텍스트를 둘러싼다. 두 번째 괄호 집합에서는 문서의 다른 곳에 저장 중인 링크를 가리키는 데 사용되는 레이블이 표시된다.

필요하지 않은 경우에도 첫 번째 대괄호 집합과 두 번째 대괄호 집합 사이에 공백을 포함할 수 있다. 두 번째 괄호 집합은 대소문자를 구분하지 않으며 문자, 숫자, 공백 또는 구두점을 포함할 수 있다.

    - [hobbit-hole][1]  
    - [hobbit-hole] [1]

<br>

## 11.5.2 Formattion the Second Part of the Link

참조 링크의 두 번째 부분은 다음 특성으로 포맷된다.

1. 대괄호로 묶인 레이블 바로 뒤에 콜론과 하나 이상의 공백이 온다.
2. 선택적으로 꺾쇠 괄호로 묶을 수 있는 링크의 URL이다.
3. 큰 따옴표, 작은 따옴표 또는 괄호로 묶을 수 있는 링크의 선택적 제목이다.

- \[1\]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
- \[1\]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
- \[1\]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'
- \[1\]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)
- \[1\]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
- \[1\]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
- \[1\]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)

링크의 두 번째 부분은 Markdown 문서 어디에나 배치할 수 있다. 일부 사용자는 나타나는 문단 바로 뒤에 배치하는 반면, 다른 사용자는 문서 끝에 배치한다. (예 : 주석 또는 각주)
