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
