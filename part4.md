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

