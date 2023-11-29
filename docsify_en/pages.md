<!-- 主文件 -->

***Initiate! Write documentation***

> ### 1. Edit the MD Document

Familiar with syntax, write content directly on the editor, and hot reload supports debugging

> Not familiar with syntax, Joplin (open source software) is recommended.

![MD语法1](../_media/_resources/MD语法1.png ':size=80%')

> Joplin supports exporting MD documents

![MD语法2](../_media/_resources/MD语法2.png ':size=50%')

> Export MD resources, copy files and images to the project, and modify the file name and image path

![MD语法3](../_media/_resources/MD语法3.png ':size=70%')

![MD语法4](../_media/_resources/MD语法4.png ':size=70%')


> ### 2. MD Syntax

Docsify supports MD syntax, please refer to:

Basic Grammar: https://markdown.com.cn/basic-syntax/i

Extended Syntax: https://markdown.com.cn/extended-syntax/


```
MD supports embedded HTML tags，\ Translated
<u>Underline</u>

1-6 # titles from large to small
### title 3

italic
*123*

bold
**123**

italic and bold
***123***

> block
>> nested blocks

1. ordered list
- unordered list
	- >> nested Unordered list
Tab keep other content aligned with the list (four spaces)

- [ ] task Block
- [x] checked

quotation mark fence
`word`
``sentence`
fence code block+syntax hint（Tab Translated）
	```python
		print('123')
	```

---  Divider, upper and lower blank lines
** * Dividers, upper and lower blank rows

Strikethrough 
~~123~~

hyperlinks
[hyperlinks](website "title")
<website>
<e-mail>
It can be used with italics, bold, and backticks

Image
![tips](path "title")

Image hyperlink
[![tips](/path "title")](URL)

Table
:- Align Left
-: Align Right
:-: Center
| Syntax |Description|
| - | - |
|Header| Title |
|Paragraph| Text |

Emojis https://gist.github.com/rxaviers/7360908
笑哭 :joy:


```


> ### 3. Docsify Supplemental Grammar

```
Emphasis on content
!> 123

General Tips
?>

The target attribute of the link
[tips](网址 ':target=_blank')
[tips](网址 ':target=_self')

Picture zooming
![tips](path ':size=WIDTHxHEIGHT') 
![tips](path ':size=50x100')
![tips](path ':size=100')
![tips](path ':size=10%')

Set picture id, class
':id=id'
':class=class'

```
