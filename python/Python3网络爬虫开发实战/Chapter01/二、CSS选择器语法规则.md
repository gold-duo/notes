### 二、CSS选择器语法规则（p17）
选择器|实例|实例描述
---|---|---
.class|.intro|选择class="intro"的所有节点
#id|#firstname|选择id="firstname"的所有节点
*|*|选择所有节点
element|p|选择所有 p 节点
element,element|div,p|选择所有 div 节点<font color='red'>和</font>所有p节点
element element|div p|选择 div 节点<font color='red'>内部的</font>所有p节点
elementselement|div>p|选择<font color='red'>父节点</font>为div节点的所有 p节点
element+element|div+p|选择紧接在 div <font color='red'>节点之后</font>的所有p节点
[attribute]|[target]|选择带有 target<font color='red'>属性</font>的所有节点
[attribute=value]|[target=blank]|选择 target="blank" 的所有 节点
[attribute~=svalue]|[title"~=flower]|选择 title <font color='red'>属性包含单词</font> flower 的所有节点
:link|a:link|选择所有未被访间的链接
:visited|a:visited|选择所有已被访问的链接
:active|a:active|选择活动链接
:hover|a:hover|选择鼠标指针位于其上的链接
:focus|input:focus|选择获得焦点的 input 节点
:first-letter|p:first-letter|选择每个p节点的首字母
:first-line|p:first-line|选择每个p 节点的首行
:first-child|p:first-child|选择属于父节点的第一个子节点的所有 P节点
:before|p:before|在每个p节点的内容之前插人内容
:after|p:after|在每个P节点的内容之后插入内容
:lang(language)|p:lang(en)|选择带有以en开头的 1ang 属性值的所有P节点
element1~element2|p~ul|选择前面有 p 节点的所有 ul 节点
[attribute^=value]|a[src^="https"]|选择 src 属性值以 https 开头的所有 a节点
[attribute$=value]|a[src$=.pdf"]|选择 src 属性值以 pdf 结尾的所有a节点
[attribute*=value]|a[src*="abc"]|选择 src 属性值中包含 abc子串的所有a节点
[:first-of-type](https://developer.mozilla.org/zh-CN/docs/Web/CSS/:first-of-type)|p:first-of-type|选择属于对父交节点的首个p节点的所有P节点
[:last-of-type](https://developer.mozilla.org/zh-CN/docs/Web/CSS/:last-of-type)|p:last-of-type|选择属于对应父节点的最后一个p节点的所有p节点
[:only-of-type](https://developer.mozilla.org/zh-CN/docs/Web/CSS/:only-of-type)|p:only-of-type|选择属于对应父节点的唯一p节点的所有p节点
:only-child|p:only-child|选择属于对应父节点的唯一子节点的所有p节点
:nth-child(n)|p:nth-child|选择属于对应父节点的第二个子节点的所有P节点
:nth-last-child(n)|p:nth-last-child|同上，不过是从最后一个子节点开始计数
:nth-of-type(n)|p:nth-of-type|选择属于对应父节点的第二个P节点的所有p节点
:nth-last-of-type(n)|p:nth-last-of-type|同上，不过是从最后一个子节点开始计数
:last-child|p:last-child|选择属于对应父节点的最后一个子节点的所有P节点
:root|:root|选择文档的根节点
:empt|p:empty|选择没有子节点的所有P节点(包括文本节点)
:target|#news:target|选择当前活动的 #news 节点
:enabled|input:enabled|选择每个启用的 input 节点
:disabled|input:disabled|选择每个禁用的 input 节点
:checked|input:checked|选择每个被选中的 input 节点
:not(selector)|:not|选择非P节点的所有节点
::selection|:selection|选择被用户选取的节点部分
