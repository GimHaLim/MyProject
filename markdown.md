# Markdown 설명서 (basic syntax ver)

## 1.1 Headings (제목)

(#) 다음에 제목을 작성한다. 사용하는 기호의 수는 제목 수준과 일치해야 한다.

| Markdown | HTML | Rendered Output |
| --- | --- | --- |
| # Heading level 1      | \<h1\>Heading level 1\</h1\> | <h1>Heading level 1</h1> |
| ## Heading level 2     | \<h2\>Heading level 2\</h2\> | <h2>Heading level 2</h2> |
| ### Heading level 3    | \<h3\>Heading level 3\</h3\> | <h3>Heading level 3</h3> |
| #### Heading level 4   | \<h4\>Heading level 4\</h4\> | <h4>Heading level 4</h4> |
| ##### Heading level 5  | \<h5\>Heading level 5\</h5\> | <h5>Heading level 5</h5> |
| ###### Heading level 6 | \<h6\>Heading level 6\</h6\> | <h6>Heading level 6</h6> |

<br>

## 1.2 Alternate Syntax (1.1 대체 문법)

제목 수준 1에 대해 # 대신 텍스트 아래 줄에 (=)를 추가한다.  
제목 수준 2에 대해 # 대신 텍스트 아래 줄에 (-)를 추가한다.  
이 때 사용되는 =, - 의 수는 상관 없다.

| Markdown                                       | Rendered Output          |
| :--------------------------------------------- | :----------------------- |
| # Heading level 1  </br> ===========           | <h1>Heading level 1</h1> |
| ## Heading level 2  </br> -------------------- | <h2>Heading level 2</h2> |

<br>

## Watch Out!

항상 (#)과 제목 이름 사이에 공백을 두어야 한다.

<br>

## 2. paragraphs (단락)

빈 줄을 사용하여 하나 이상의 텍스트 행을 구분한다. 즉, enter을 2회 사용하면 된다.

| Markdown | HTML | Rendered Output |
| --- | --- | --- |
| I really like using Markdown. | \<p\>I really like using Markdown.\</p\> | <p>I really like using Markdown.</p> |
| I think I'll use it to format all of my doucuments from now on. | \<p\>I think I'll use it to format all of my doucuments from now on.\</p\> | <p>I think I'll use it to format all of my doucuments from now on.</p> |

<br>

## Don't do this!

공백이나 탭으로 단락을 들여서는 안된다.

<br>

## 3. Line Breaks (줄바꿈) 

두 개 이상의 공백으로 줄을 끝낸다.

| Markdown | HTML | Rendered Output |
| --- | --- | --- |
| This is the first line.<br>And this is the second line. | \<p\>This is the first line. \<br\> And this is the second line.\</p\> | <p>This is the first line. <br> And this is the second line.</p> |

<br>

## Add!

하지만 이 방법은 공간을 보기 어렵고, 많은 사람들이 실수를 하는 경우가 있기 때문에 다른 방법으로 거의 모든 Markdown 애플리케이션에서 \<br\> HTML tag를 지원하고 있다.

<br>

## Don't do this!

First line with a backslash after.\ And the next line. = ( \ ) 사용  
Fisrt line with nothing after. And the next line. = 공백 없음

<br>

## 4.1 Emphasis (강조) 

텍스트를 굵게 또는 기울임꼴로 만들어 강조 표시를 추가할 수 있다.

<br>

## 4.2 **BOLD**

단어 또는 구 앞뒤에 두 개의 별표 또는 밑줄을 추가한다.  
강조하기 위해 단어의 가운데를 굵게 표시하려면 문자 주위에 공백 없이 두 개의 별표를 추가한다.

| Markdown | HTML | Rendered Output |
| --- | --- | --- |
| I just love ** bold text **. | I just love \<strong\>bold text\</strong\>. | I just love <strong>bold text</strong>. |
| I just love __ bold text __. | I just love \<strong\>bold text\</strong\>. | I just love <strong>bold text</strong>. |
| Love\*\*is\*\*bold | Love\<strong\>is\</strong\>bold | Love<strong>is</strong>bold |

<br>

## Don't do this!

Markdown 응용프로그램은 단어의 중간에 밑줄을 처리하는 방법에 동의하지 않고, 호환성을 위해 별표로 단어의 중간을 bold로 강조표시한다.

Love__is__bold (x)

<br>

## 4.3 *ITALIC*

단어 또는 구 앞뒤에 하나의 별표 또는 밑줄을 추가한다.  
강조하기 위해 단어의 중간을 기울임꼴로 표시하려면 문자 주위에 공백 없이 별표 하나를 추가한다.

| Markdown | HTML | Rendered Output |
| --- | --- | --- |
| Italicized text is the * cat's meow *. | Italicized text is the \<em\>cat's meow\</em\>. | Italicized text is the <em>cat's meow</em>. |
| Italicized text is the _ cat's meow _. | Italicized text is the \<em\>cat's meow\</em\>. | Italicized text is the <em>cat's meow</em>. |
| A \*cat\* meow | A\<em\>cat\</em\>meow | A<em>cat</em>meow |

<br>

## Don't do this!

Markdown 응용프로그램은 단어의 중간에 밑줄을 처리하는 방법에 동의하지 않는다. 호환성을 위해 별표를 사용하여 단어 가운데를 기울임꼴로 강조해야 한다.

A_cat_meow (x)

<br>

## 4.4 __*BOLD and ITALIC*__

bold와 italic을 동시에 사용하여 강조하려면 단어 또는 구 앞뒤에 세 개의 별표 또는 밑줄을 추가한다.  
강조하기 위해 단어의 가운데를 굵고 기울임꼴로 표시하려면 문자 주위에 공백 없이 세 개의 별표를 추가한다.

이 때 별표와 밑줄을 혼합해서 사용할 수 있다. 하지만 별과 밑줄의 배치가 가운데를 중심으로 대칭으로 이루어져야 사용 가능하다. 예를 들어, (\_\*\*)로 시작한다면 (\*\*\_)로 끝나야 한다.

<br>

## Don't do this!

Markdown 응용프로그램은 단어의 중간에 밑줄을 처리하는 방법에 동의하지 않으므로 호환성을 위해 가운데 단어를 Bold와 Italic으로 강조할 때 별표를 사용해야 한다.

<br>

## 5.1 Blockquotes (인용구)

단락 앞에 (>)를 추가한다.

    > Dorothy followed her through many of the beautiful rooms in her castle.

### The rendered output looks like this :

> Dorothy followed her through many of the beautiful rooms in her castle.

<br>

## 5.2 Blockquotes whit Multiple Paragraphs (여러 문단이 있는 인용구)

Blockquotes는 문단 사이의 빈 줄에 (>)를 추가하여 여러 단락을 포함할 수 있다. 

    > Dorothy followed her through many of the beautiful rooms in her castle.
    >
    > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### The rendered output looks like this :

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

<br>

## 5.3 Nested Blockquotes (내포된 인용구)

인용구 안에 인용구가 다시 내포될 수 있다. 내포하고 싶은 구문 앞에 \>\>를 추가한다.

    > Dorothy followed her through many of the beautiful rooms in her castle.
    >
    >> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### The rendered output looks like this :

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

<br>

## 5.4 Blockquotes with Other Elements (다른 요소들이 있는 인용구)

인용구는 다른 Markdown 형식 요소를 포함할 수 있다. 모든 요소를 사용할 수 있는 것은 아니므로 어떤 요소가 작동하는지 실험해보고 사용해야 한다.

예시 :

    > #### The quarterly results look great!
    >
    > - Revenue was off the chart.
    > - Profits were higher than ever.
    >
    >  *Everything* is going according to **plan**.

### The rendered output looks like this :

> ### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
> *Everythinh* is going according to **plan**.

<br>

## 6.1 List (목록)

항목을 순서 목록과 순서 없는 목록으로 구성할 수 있다.

<br>

## 6.2 Ordered Lists (순서 목록)

숫자 뒤에 마침표가 있는 줄 항목을 추가해야 한다. 이 때, 목록이 숫자 1로 시작한다면, 나머지는 순서대로 나열할 필요없다.

    1. First item
    8. Second item
    3. Third item
    5. Fourth item

### The rendered output looks like this :  

1. First item
8. Second item
3. Third item
5. Fourth item

<br>

## 6.3 Unordered Lists (순서 없는 목록)

정렬되지 않은 목록을 만들려면 줄 항목 앞에 (-), (*) 또는 (+) 기호를 추가한다. 하나 이상의 학목을 들여써 중첩 목록을 작성할 수 있다. (여기에서 중첩 목록을 작성하는 법은 6.4에 나온다.)

    * First item
    * Second item
    * Third item
    * Fourth item

### The rendered output looks like this : 

* First item
* Second item
* Third item
* Fourth item

<br>

## Don't do this!

Markdown 응용프로그램은 동일한 목록에서 다른 기호를 처리하는 방법에 동의하지 않으므로 호환성을 위해 같은 목록에 있는 구분 기호를 혼합하지 않도록 주의해야 한다.

    + First item
    * Second item
    - Third item

### The rendered output looks like this : 

+ First item
* Second item
- Third item

이 세 가지는 모두 다른 항목이 된다.

<br>

## 6.4 Adding Elements in Lists (목록에 요소 추가하기)

목록의 연속성을 유지하면서 목록에 다른 요소를 추가하려면 다음 예와 같이 요소를 네 칸 또는 한 탭으로 들여쓴다.

<br>

> ### 요소 1 : paragraphs

    + THis is he first list item.
    + Here's the second list item.  
        I need to add another paragraph below the second list item.
    + And here's the third list item. 

### The rendered output looks like this : 

+ THis is he first list item.
+ Here's the second list item.  
    I need to add another paragraph below the second list item.
+ And here's the third list item. 

<br>

> ### 요소 2 : Blockquotes

    + THis is he first list item.
    + Here's the second list item.  
        > A blockquote would look great below the second list item.
    + And here's the third list item. 

### The rendered output looks like this : 

+ THis is he first list item.
+ Here's the second list item.  
    > A blockquote would look great below the second list item.
+ And here's the third list item. 

<br>

> ### 요소 3 : Code Blocks

코드 블록은 일반적으로 네 개의 공백 또는 하나의 탭으로 들여쓰기 된다. 목록에 있으면 8칸 또는 두 탭을 들여쓴다.

    1.  Open the file.
    2.  Find the following code block on line 21:

            <html>
              <head>
                <title>Test</title>
              </head>

    3.  Update the title to match the name of your website.

### The rendered output looks like this : 

1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.

<br>

> ### 요소 4 : Images

    1. Open the file containing the Linux mascot.
    2. Marvel at its beauty.
       
        ![Tux, the Linux mascot](https://d33wubrfki0l68.cloudfront.net/e7ed9fe4bafe46e275c807d63591f85f9ab246ba/e2d28/assets/images/tux.png)
        
    3. Close the file.

### The rendered output looks like this : 

1. Open the file containing the Linux mascot.
2. Marvel at its beauty.
   
    ![Tux, the Linux mascot](https://d33wubrfki0l68.cloudfront.net/e7ed9fe4bafe46e275c807d63591f85f9ab246ba/e2d28/assets/images/tux.png)

3. Close the file.

<br>

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

<br>

## 11.6 An Example Putting the Parts Together

URL을 문단에 표준 URL 링크로 추가하면 다음과 같이 표시된다.

    In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, a bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole][1], and that means comfort.
    
    [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbitt lifestyles"

### The rendered output looks like this:

In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, a bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole][1], and that means comfort.
    
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbitt lifestyles"

### The HTML for the link would be:

    <a href="https://en.wikipedia.org/wiki/Hobbit#Lifestyle" title="Hobbit lifestyles">hobbit-hole</a>

<br>

## 12.1 Images (이미지)

이미지를 추가하려면 느낌표를 추가하고 대괄호 안에 대체 텍스트를 추가하고 괄호 안에 이미지의 경로 또는 URL을 추가한다. 선택적으로 괄호 안의 URL 뒤에 제목을 추가할 수 있다.

    ![벚꽃은 정말 아름다워요!](https://www.jobaba.net/file/image.do?filePath=sONy7CFJVlHd+/JjdwFq+iS2HVEsSAv5J9kJDk6VJNWWtcEaYTwOm11GhF32XM4L "벚꽃")

The rendered output looks like this:

![벚꽃은 정말 아름다워요!](https://www.jobaba.net/file/image.do?filePath=sONy7CFJVlHd+/JjdwFq+iS2HVEsSAv5J9kJDk6VJNWWtcEaYTwOm11GhF32XM4L "벚꽃")

## 12.2 Linking Images

이미지에 링크를 추가하려면 이미지에 대한 표시줄을 대괄호로 묶은 다음 괄호 안에 링크를 추가한다.

    [![An old rock in the desert](https://d33wubrfki0l68.cloudfront.net/70a143fdf134aacde3740662a2a47a2a1ee0d216/276c9/assets/images/shiprock.jpg "Shiprock, New Mexico by BEAU rogers")](https://www.youtube.com/)

### The rendered output looks like this:

[![An old rock in the desert](https://d33wubrfki0l68.cloudfront.net/70a143fdf134aacde3740662a2a47a2a1ee0d216/276c9/assets/images/shiprock.jpg "Shiprock, New Mexico by BEAU rogers")](https://www.youtube.com/)

<br>

## 13.1 Escaping Characters (이스케이핑 문자)

Markdown 문서에서 텍스트 서식을 지정하는 데 사용할 literal 문자를 표시하려면 문자 앞에 백슬래시를 추가한다.

    \* Without the backslash, this would be a bullet in an unordered list.

### The rendered output looks like this:

\* Without the backslash, this would be a bullet in an unordered list.

<br>

## 13.2 Characters You Can Escape (이스케이프 할 수 있는 문자)

| character | name             |
| --------- | ---------------- |
| \\        | backslash        |
| \`        | backtick         |
| \*        | asterissk        |
| \_        | underscore       |
| \{\}      | curly braces     |
| \[\]      | brackets         |
| \<\>      | angle brackets   |
| \(\)      | parentheses      |
| \#        | pound sign       |
| \+        | pls sign         |
| \-        | minus sign       |
| \.        | dot              |
| \!        | exclamation mark |
| \|        | pipe             |

<br>

## 14. HTML

많은 Markdown 응용 프로그램들에서 HTML 태그를 사용할 수 있다. 이 기능은 Markdown stntax보다 특정 HTML 태그를 선호하는 경우에 유용하다. 예를 들어, 일부 사람들은 이미지에 HTML 태그를 사용하는 것이 더 쉽다고 생각한다. HTML을 사용하면 텍스트 색상을 지정하거나 이미지의 너비를 변경하는 등 요소의 속성을 변경해야 할 때도 유용하다.

HTML을 사용하려면 Markdown 형식 파일의 택스트에 태그를 배치하면 된다. 

    This **word** is bold. This <em>word</em> is italic.

### The rendered output looks like this:

This **word** is bold. This <em>word</em> is italic.

<br>

## Watch Out! :

보안상의 이유로 일부 Markdown 응용프로그램이 HTML을 지원하지 않는다. 확실하지 않은 경우 Markdown 프로그램의 설명서를 확인하면 된다. 

빈 줄을 사용하는 블록 레벨 HTML 요소는 주변 컨텐츠에서 분리해야 한다. 형식 지정에 방해가 될 수 있는 탭이나 공백으로 들어쓰지 않는다. 

블록 수준 태그 내부에서는 Markdown 구문을 사용할 수 없다.

<br>
<br>

# GitHub repository URL

My GitHub repsitory URL is [here](https://github.com/GimHaLim/Practice.git "GitHub repository").
