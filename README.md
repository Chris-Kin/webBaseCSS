# 关于项目
- 适用场景：使用了基于js框架（如vue、react、angular等）开发的UI库（如ant-design,element,iview等）的web系统
- 功能：提供统一易用的基础样式类库，以减少在项目开发中编写冗余css，并实现UI界面的整体一致性
- 不同于其他css库，本项目遵从最小颗粒样式原则，你可以自由组合类名以达到复合样式展现的目的
- 项目内部引入normalize.css库，以解决现代html元素在各个浏览器端表现不一的问题

# 类名的命名规则：
> 总原则：面向属性命名、对开发者透明且有表现意义、所有字母均小写，单个中划线作为辅助

|分类|规则|示例|
|:--:|:--|:--|
| 属性值为数字类型的类名命名规则 | 数值与属性之间不加中划线 | ```m10 —> margin: 10px```<br />```mr10 —> margin-right: 10px```<br />```pt40 -> padding-top: 40px```<br />```w80 -> width: 80px``` |
| 属性值为非数字类型的类名命名规则 | 属性名首字母缩写-属性值单词首字母缩写 | ```dis-ib -> display: inline-block```<br />```ta-c -> text-align: center```<br /> ```td-ol -> text-decoration: overline```|
| .. | .. |..|
|首字母简写有歧义的属性命名| 采用属性名单词缩写形式命名 | ```dis-ib -> display: inline-block``` |

# 使用介绍
1. 全局引入webBaseCSS： ```import 'webBaseCSS/dist/index.css';```
2. 在需要设置样式的标签上定义类，如``` <div class="mt10 w200"></div>``` 表示对div设置```margin-top: 10px; width: 200px```
3. [normalize.css](https://necolas.github.io/normalize.css/)
