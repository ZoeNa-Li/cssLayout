# CSS布局
>>该库主要对CSS布局进行代码演示，一共分为7章节
### 水平布局

>>水平居中的页面布局中最为常见的一种布局形式，多出现于标题，以及内容区域的组织形式，包括以下六种方法
- text-align: center 文本水平居中
- display:table; 文本/盒子 水平居中
- 指定宽度  margin: 0 auto;盒子水平居中
- position: absolute;水平居中
- flex+justify-content: center;水平居中
- 父flex + 子margin: 0 auto;水平居中

### 垂直居中布局

- line-height = 容器高度
- display: table-cell;+ vertical-align: middle; 文本+盒子在父容器中垂直居中
- display:inline-block;+vertical-align:middle;+line-height
-  绝对定位，一个盒子在另一个盒子中垂直居中
- flex布局，一个盒子在另一个盒子中垂直居中

### 多列布局

#### 左侧定宽右侧自适应
- float + margin 同时注意IE6下 3px bug
- float + overflow 
- flex
#### 两列定宽，一列自适应
- float + margin 
- float + overflow 
- flex
- table
#### 两侧定宽，中间自适应
- float
- 中间flex:1
#### 一列不定宽，一列自适应
- flex
- float + overflow:hidden
#### 多列等宽
- 父，dispaly:flex; 子，flex:1;

### 自适应布局

- 设置布局宽度等于设备宽度，布局viewport等于度量viewport

### stacky-footer布局

- stacky-footer布局让footer组件自动定位到页面最底部，解决方案有以下两种

#### 方案一：padding-bottom+margin负值
- 上面内容的padding-bottom:footer高; ，footer的margin: -footer高 auto;
#### 方案二：flex
- display: flex;flex-flow: column;  内容盒子：flex: 1;  footer: 设置高度
