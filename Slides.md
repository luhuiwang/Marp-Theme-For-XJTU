---
marp: true
theme: default
paginate: true
footer: 2021年5月17日
style: |
  :root {
    font-family: Noto Sans SC;
    background-color: white;
  } 
  section footer{ 
      font-size: 30px; 
      display: none; 
      position: absolute;
      text-align: center;
      width: 100%;
      color: black;
      font-weight: bold;
  } 
  section h1 {color:DarkRed}
  section {
    background-image:url('./img/background.png'),url('./img/logo.png');
    background-position: bottom right, right 3% top 3%;
    background-repeat: no-repeat,no-repeat;
    background-size: 60%,30%;
  }
  strong,em {
    color: brown ;
  }
  section::after {
    font-weight: bold;
    color: black;
    content:  attr(data-marpit-pagination) ' / ' attr(data-marpit-pagination-total);
  }

  

size: 16:9
# size: 4:3
---
<style scoped>
section h1 {text-align: center;font-size: 80px}
section h2 {padding-bottom: 8%;text-align: center;font-size: 40px}
section p {text-align: center;font-size: 40px;font-weight:bold}

footer{ display: block } 
</style>

# Marp幻灯片模板

## 作者：XXX

西安交通大学
计算机科学与技术学院

---

<style scoped>
li {font-size: 40px;font-weight:bold;}
</style>

# 总览

1. 如何使用
2. 首页修改
3. 背景修改
4. 图片格式
5. 左右排布
6. CSS 说明

---

# 如何使用 Marp 制作组会 Slides

1. 下载 VS code
2. 在插件中心安装Marp for VS Code
3. 新建一个 md 文件,复制 1~51 行 CSS 或者从该模板中直接新建.
4. 点击 1 可以实时显示 Slides,点击 2 选择 export 可以导出 PDF.
   ![w:10cm](https://cy-1256894686.cos.ap-beijing.myqcloud.com/20201129171243.png)

---

# 首页修改

我预设了适合*展示*的标题大小,当然如果是需要修改适合投影的字体大小可在源代码中第 12 行修改`h1的font-size`.

改变`background-image:url('./img/background.png');`可以修改首页背景图片.

```css
<style scoped>
section h1 {text-align: center;font-size: 80px;color:black;}
section {
  background-image:url('./img/background.png');
  background-size:cover
}
footer{color:black;font-size: 20px;} 
</style>
```

---

# 背景修改

**修改模板**源代码 27~31 行`background-image:url('./img/background.png');`中背景图片即可.

```css
section{
  background-image:url('./img/background.png');
  background-size:cover;
  position: absolute;
  }
```

---

# 字体修改

全局格式修改在源代码 31~35 行

`h1`一级大标题
`h2`二级大标题
`p`正文字体
`table`表格字体,居中
`li`列表字体,居左

```css
section h1 {font-size:40px;color:black;margin-top:px;}
section h2 {font-size:30px;color:black;margin-top:px;}
section p {font-size: 25px;color:black;}
section table {text-align: center;font-size: 32px;color:black;}
section a {font-size: 25px;color:black;}
li {font-size: 30px;text-align: left;}
```

---

# 图片格式

默认居中,~~临时~~在某一slides中修改可以

```css
<style scoped>
img {
    margin-left: auto; margin-right:auto; 
    display:block;margin:0 auto;width:25cm;
    }
</style>
或者:
![w:2cm h:2cm](background.png)
```

![w:2cm h:2cm](background.png)

---

# 左右排布

```
![bg left:40% w:5cm h:5cm](background.png)
```

![bg left:40% w:5cm h:5cm](background.png)

---

# 左右排布

```
![bg right:40% w:5cm h:5cm](background.png)
```

![bg right:40% w:5cm h:5cm](background.png)

---

# CSS 说明

```
https://www.w3school.com.cn/css/css_image_gallery.asp

https://marpit.marp.app/theme-css
```

# 更多细节

```
https://marpit.marp.app/usage
```

# 更多Markdown 语法

```
https://www.markdown.xyz/basic-syntax/
```

---

<style scoped>
section h1 {text-align: center;font-size: 80px}
</style>

<!-- _class: lead gaia -->

# 谢谢大家，

# 欢迎提问！
