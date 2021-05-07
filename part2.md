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
