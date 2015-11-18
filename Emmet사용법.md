# Emmet - a Must tool for HTML/CSS coder

Emmet 은 기본적으로 에디터 자동 완성 툴이다. 
에디터가 HTML 또는 CSS 스타일쉬트 문서로 인식하는 환경에서만 동작한다. 
Sublime Text 혹은 Atom 사용자는 Emmet Package를 설치한다. 

**사용법**: 명령어(예: !, doc, a, html, .example)를 입력한 후 <Tab>으로 실행한다

## Emmet Meta Characters
  - > : 해당 태그를 열고 들여쓰기를 한다.
  - + : 줄바꿈을 하고 다음 태그를 추가한다.
  - . : class를 지정한다.
  - # : id를 지정한다.
  - [] : 커스텀 속성을 지정한다. .
  - ^ : 한 수준 올라간다.
  - () : 그룹을 지정한다.
  - * : 곱하기로 정해진 수만큼 태그를 반복한다

## Examples
**!**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

**html:5**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

**link** 

``` <link rel="stylesheet" href=""> ```

**html**

``` <html></html> ```

**a** 

``` <a href=""></a> ```

**img**

``` <img src="" alt=""> ```

## More examples
### > 들여쓰기, * 반복하기 - ul Tag를 생성하고, li 들여기 3회 반복
```
ul>li*3
<ul>
    <li></li>
    <li></li>
    <li></li>
</ul>
```

### . class를 생성하고 자동으로 div tag가 자동으로 입력된다
```
.example
<div class="example"></div>

div.example
<div class="example"></div>
```

### # id를 생성하고 자동으로 div tag가 자동으로 입력된다
```
#example
<div id="example"></div>

div#example
<div id="example"></div>
```

### + 같은 수준의 sibling tag를 생성
```
h1+p.bright
<h1></h1>
<p class="bright"></p>
```

### h1 Tag 만들고, 줄바꿈하여 ul Tag만들고, 들여쓰기 하여 li 3회 반복
```
h1+ul>li*3  
<h1></h1>
<ul>
    <li></li>
    <li></li>
    <li></li>
</ul>
```

### > 들여쓰기, + 같은 수준, ^ 한 수준 up, () 한 그룹으로 지정
```
p>img+p
<p>
    <img src="" alt="">
    <p></p>
</p>

p>img^p
<p>
    <imag></imag>
</p>
<p></p>

(p>img)+p
<p><img src="" alt=""></p>
<p></p>
```
### $ 숫자를 채워넣음
```
ul>li.item$*3
<ul>
    <li class="item1"></li>
    <li class="item2"></li>
    <li class="item3"></li>
</ul>
```

### dummy text - lorem ipsum
```
lorem
Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
Corrupti, fuga voluptatibus, possimus repellendus aspernatur 
placeat quibusdam facilis cum labore! Repellat voluptates vero 
perspiciatis maxime earum, voluptatum veniam quidem dicta nobis.
```
