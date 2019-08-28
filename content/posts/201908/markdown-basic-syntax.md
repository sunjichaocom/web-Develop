---
title: "Markdown基本语法"
date: 2019-08-28T12:10:30+08:00
draft: false
tags:
    - Markdown
---

>笨脑瓜总记不住，整理一下以后常用

## 1. 标题

在想要设置为标题的文字前面加`#`来表示

一个`#`是一级标题，二个`#`是二级标题，以此类推。支持六级标题。

`示例：`

```markdown
# 这是一级标题
## 这是二级标题
### 这是三级标题
#### 这是四级标题
##### 这是五级标题
###### 这是六级标题
```

`效果如下：`

# 这是一级标题
## 这是二级标题
### 这是三级标题
#### 这是四级标题
##### 这是五级标题
###### 这是六级标题

## 2. 字体

* 加粗

    要加粗的文字左右分别用两个`*`号包起来

* 斜体

    要倾斜的文字左右分别用一个`*`号包起来

* 斜体加粗

    要倾斜和加粗的文字左右分别用三个`*`号包起来

* 删除线

    要加删除线的文字左右分别用两个`~~`号包起来

`示例：`

```markdown
**这是加粗的文字**
*这是倾斜的文字*
***这是斜体加粗的文字***
~~这是加删除线的文字~~
```

`效果如下：`

**这是加粗的文字**

*这是倾斜的文字*

***这是斜体加粗的文字***

~~这是加删除线的文字~~

## 3. 引用

在引用的文字前加>即可。引用也可以嵌套，如加两个>>三个>>>

`示例：`

```markdown
>这是引用的内容
>>这是引用的内容
>>>>>>>>>>这是引用的内容
```

`效果如下：`

>这是引用的内容
>>这是引用的内容
>>>>>>>>>>这是引用的内容

## 4. 分割线

三个或者三个以上的 - 或者 * 都可以。

`示例：`

```markdown
---
----
***
*****
```

`效果如下：`

---
----
***
*****

## 5. 图片

`语法：`

```markdown
![图片alt](图片地址 "图片title")

图片alt就是显示在图片下面的文字，相当于对图片内容的解释。
图片title是图片的标题，当鼠标移到图片上时显示的内容。title可加可不加
```

`示例：`

```markdown
![Sun](https://avatars2.githubusercontent.com/u/21169748?v=4&s=300 "Sun")
```

`效果如下：`

![Sun](https://avatars2.githubusercontent.com/u/21169748?v=4&s=300 "Sun")

## 6. 超链接

`语法：`

```markdown
[超链接名](超链接地址 "超链接title")
title可加可不加
```

`示例：`

```markdown
[Github](https://github.com)
[Coding](https://coding.net)
```

`效果如下：`

[Github](https://github.com)

[Coding](https://coding.net)

## 7. 列表

* 无序列表

    `语法：`

    ```markdown
    无序列表用 - + * 任何一种都可以
    ```

    `示例：`

    ```markdown
    - 列表内容
    + 列表内容
    * 列表内容

    注意：- + * 跟内容之间都要有一个空格
    ```

    `效果如下：`

    - 列表内容
    + 列表内容
    * 列表内容

* 有序列表

    `语法：`

    ```markdown
    数字加点
    注意：序号跟内容之间要有空格
    ```

    `示例：`

    ```markdown
    1. 列表内容
    2. 列表内容
    3. 列表内容
    ```

    `效果如下：`

    1. 列表内容
    2. 列表内容
    3. 列表内容

* 列表嵌套

    `语法：`

    ```markdown
    上一级和下一级之间敲三个空格即可
    注意：关于嵌套部分我有点蒙，有说三个空格的，有说四个空格的，也有说两个Tab的。
    ```

    `示例：`

    ```markdown
    1. one
        1. one-1
        2. one-2
    2. two
        * two-1
        * two-2
    ```

    `效果如下：`

    1. one
        1. one-1
        2. one-2
    2. two
        * two-1
        * two-2

## 8. 表格

`语法：`

```markdown
表头|表头|表头
---|:--:|---:
内容|内容|内容
内容|内容|内容

第二行分割表头和内容。
- 有一个就行，为了对齐，多加了几个
文字默认居左
-两边加：表示文字居中
-右边加：表示文字居右
注：原生的语法两边都要用 | 包起来。此处省略
```

`示例：`

```markdown
排行|绰号
---|:--:
老大|一招就死
老二|非死不可
老三|死缠烂打
老四|永远不死
```

`效果如下：`

排行|绰号
---|:--:
老大|一招就死
老二|非死不可
老三|死缠烂打
老四|永远不死

## 9. 代码

`示例：`


    ```javascript
    var num = 0;
    for (var i = 0; i < 5; i++) {
        num+=i;
    }
    console.log(num);
    ```


`效果如下：`

```javascript
var num = 0;
for (var i = 0; i < 5; i++) {
    num+=i;
}
console.log(num);
```

`支持语法列表：`

| 语法名 | 简写 |
|:---|:---|
| 1C                      | 1c                                                |
| ABNF                    | abnf                                              |
| Access logs             | accesslog                                         |
| Ada                     | ada                                               |
| ARM assembler           | armasm, arm                                       |
| AVR assembler           | avrasm                                            |
| ActionScript            | actionscript, as                                  |
| Apache                  | apache, apacheconf                                |
| AppleScript             | applescript, osascript                            |
| AsciiDoc                | asciidoc, adoc                                    |
| AspectJ                 | aspectj                                           |
| AutoHotkey              | autohotkey                                        |
| AutoIt                  | autoit                                            |
| Awk                     | awk, mawk, nawk, gawk                             |
| Axapta                  | axapta                                            |
| Bash                    | bash, sh, zsh                                     |
| Basic                   | basic                                             |
| BNF                     | bnf                                               |
| Brainfuck               | brainfuck, bf                                     |
| C#                      | cs, csharp                                        |
| C++                     | cpp, c, cc, h, c++, h++, hpp                      |
| C/AL                    | cal                                               |
| Cache Object Script     | cos, cls                                          |
| CMake                   | cmake, cmake.in                                   |
| Coq                     | coq                                               |
| CSP                     | csp                                               |
| CSS                     | css                                               |
| Cap’n Proto            | capnproto, capnp                                  |
| Clojure                 | clojure, clj                                      |
| CoffeeScript            | coffeescript, coffee, cson, iced                  |
| Crmsh                   | crmsh, crm, pcmk                                  |
| Crystal                 | crystal, cr                                       |
| D                       | d                                                 |
| DNS Zone file           | dns, zone, bind                                   |
| DOS                     | dos, bat, cmd                                     |
| Dart                    | dart                                              |
| Delphi                  | delphi, dpr, dfm, pas, pascal, freepascal, lazarus, lpr, lfm |
| Diff                    | diff, patch                                       |
| Django                  | django, jinja                                     |
| Dockerfile              | dockerfile, docker                                |
| dsconfig                | dsconfig                                          |
| DTS (Device Tree)       | dts                                               |
| Dust                    | dust, dst                                         |
| EBNF                    | ebnf                                              |
| Elixir                  | elixir                                            |
| Elm                     | elm                                               |
| Erlang                  | erlang, erl                                       |
| Excel                   | excel, xls, xlsx                                  |
| F#                      | fsharp, fs                                        |
| FIX                     | fix                                               |
| Fortran                 | fortran, f90, f95                                 |
| G-Code                  | gcode, nc                                         |
| Gams                    | gams, gms                                         |
| GAUSS                   | gauss, gss                                        |
| Gherkin                 | gherkin                                           |
| Go                      | go, golang                                        |
| Golo                    | golo, gololang                                    |
| Gradle                  | gradle                                            |
| Groovy                  | groovy                                            |
| HTML, XML               | xml, html, xhtml, rss, atom, xjb, xsd, xsl, plist |
| HTTP                    | http, https                                       |
| Haml                    | haml                                              |
| Handlebars              | handlebars, hbs, html.hbs, html.handlebars        |
| Haskell                 | haskell, hs                                       |
| Haxe                    | haxe, hx                                          |
| Hy                      | hy, hylang                                        |
| Ini                     | ini                                               |
| Inform7                 | inform7, i7                                       |
| IRPF90                  | irpf90                                            |
| JSON                    | json                                              |
| Java                    | java, jsp                                         |
| JavaScript              | javascript, js, jsx                               |
| Leaf                    | leaf                                              |
| Lasso                   | lasso, ls, lassoscript                            |
| Less                    | less                                              |
| LDIF                    | ldif                                              |
| Lisp                    | lisp                                              |
| LiveCode Server         | livecodeserver                                    |
| LiveScript              | livescript, ls                                    |
| Lua                     | lua                                               |
| Makefile                | makefile, mk, mak                                 |
| Markdown                | markdown, md, mkdown, mkd                         |
| Mathematica             | mathematica, mma                                  |
| Matlab                  | matlab                                            |
| Maxima                  | maxima                                            |
| Maya Embedded Language  | mel                                               |
| Mercury                 | mercury                                           |
| Mizar                   | mizar                                             |
| Mojolicious             | mojolicious                                       |
| Monkey                  | monkey                                            |
| Moonscript              | moonscript, moon                                  |
| N1QL                    | n1ql                                              |
| NSIS                    | nsis                                              |
| Nginx                   | nginx, nginxconf                                  |
| Nimrod                  | nimrod, nim                                       |
| Nix                     | nix                                               |
| OCaml                   | ocaml, ml                                         |
| Objective C             | objectivec, mm, objc, obj-c                       |
| OpenGL Shading Language | glsl                                              |
| OpenSCAD                | openscad, scad                                    |
| Oracle Rules Language   | ruleslanguage                                     |
| Oxygene                 | oxygene                                           |
| PF                      | pf, pf.conf                                       |
| PHP                     | php, php3, php4, php5, php6                       |
| Parser3                 | parser3                                           |
| Perl                    | perl, pl, pm                                      |
| Pony                    | pony                                              |
| PowerShell              | powershell, ps                                    |
| Processing              | processing                                        |
| Prolog                  | prolog                                            |
| Protocol Buffers        | protobuf                                          |
| Puppet                  | puppet, pp                                        |
| Python                  | python, py, gyp                                   |
| Python profiler results | profile                                           |
| Q                       | k, kdb                                            |
| QML                     | qml                                               |
| R                       | r                                                 |
| RenderMan RIB           | rib                                               |
| RenderMan RSL           | rsl                                               |
| Roboconf                | graph, instances                                  |
| Ruby                    | ruby, rb, gemspec, podspec, thor, irb             |
| Rust                    | rust, rs                                          |
| SCSS                    | scss                                              |
| SQL                     | sql                                               |
| STEP Part 21            | p21, step, stp                                    |
| Scala                   | scala                                             |
| Scheme                  | scheme                                            |
| Scilab                  | scilab, sci                                       |
| Shell                   | shell, console                                    |
| Smali                   | smali                                             |
| Smalltalk               | smalltalk, st                                     |
| Stan                    | stan                                              |
| Stata                   | stata                                             |
| Stylus                  | stylus, styl                                      |
| SubUnit                 | subunit                                           |
| Swift                   | swift                                             |
| Test Anything Protocol  | tap                                               |
| Tcl                     | tcl, tk                                           |
| TeX                     | tex                                               |
| Thrift                  | thrift                                            |
| TP                      | tp                                                |
| Twig                    | twig, craftcms                                    |
| TypeScript              | typescript, ts                                    |
| VB.Net                  | vbnet, vb                                         |
| VBScript                | vbscript, vbs                                     |
| VHDL                    | vhdl                                              |
| Vala                    | vala                                              |
| Verilog                 | verilog, v                                        |
| Vim Script              | vim                                               |
| x86 Assembly            | x86asm                                            |
| XL                      | xl, tao                                           |
| XQuery                  | xpath, xq                                         |
| Zephir                  | zephir, zep                                       |


## 10. 流程图

`示例：`

```markdown
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End:>http://www.google.com
op1=>operation: My Operation|past
op2=>operation: Stuff|current
sub1=>subroutine: My Subroutine|invalid
cond=>condition: Yes
or No?|approved:>http://www.google.com
c2=>condition: Good idea|rejected
io=>inputoutput: catch something...|request

st->op1(right)->cond
cond(yes, right)->c2
cond(no)->sub1(left)->op1
c2(yes)->io->e
c2(no)->op2->e
```

`效果如下：`

```flow
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End:>http://www.google.com
op1=>operation: My Operation|past
op2=>operation: Stuff|current
sub1=>subroutine: My Subroutine|invalid
cond=>condition: Yes
or No?|approved:>http://www.google.com
c2=>condition: Good idea|rejected
io=>inputoutput: catch something...|request

st->op1(right)->cond
cond(yes, right)->c2
cond(no)->sub1(left)->op1
c2(yes)->io->e
c2(no)->op2->e
```


#添加下面代码
<div class="mermaid">
graph LR
    A --- B
    B-->C[fa:fa-ban forbidden]
    B-->D(fa:fa-spinner);


