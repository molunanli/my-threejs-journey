**目标：** 为 Three.js 学习项目创建一个 GitHub 仓库，并启用 GitHub Pages 功能，实现代码托管和在线 Demo 自动部署。

**日期：** `**2025年07月05日**`

<h2 id="cc22183c"><font style="color:rgb(64, 64, 64);">一、</font>在 GitHub 上创建新仓库</h2>
1. **<font style="color:rgb(64, 64, 64);">登录 GitHub：</font>**<font style="color:rgb(64, 64, 64);"> </font><font style="color:rgb(64, 64, 64);">访问</font><font style="color:rgb(64, 64, 64);"> </font>[<font style="color:rgb(59, 130, 246);">https://github.com/</font>](https://github.com/)<font style="color:rgb(64, 64, 64);"> </font><font style="color:rgb(64, 64, 64);">并登录。</font>
2. **<font style="color:rgb(64, 64, 64);">创建新仓库：</font>**
    1. <font style="color:rgb(64, 64, 64);">点击右上角 </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">+</font>**`<font style="color:rgb(64, 64, 64);"> 图标 -> </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">New repository</font>**`<font style="color:rgb(64, 64, 64);">。</font>
    2. <font style="color:rgb(64, 64, 64);">填写仓库信息：</font>
        1. **<font style="color:rgb(64, 64, 64);">Repository name:</font>**<font style="color:rgb(64, 64, 64);"> </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">my-threejs-journey</font>**`<font style="color:rgb(64, 64, 64);"> </font>
        2. **<font style="color:rgb(64, 64, 64);">Description:</font>**<font style="color:rgb(64, 64, 64);"> </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">我学习Threejs的过程记录，包括代码和我的笔记</font>**`<font style="color:rgb(64, 64, 64);"> (可选，描述仓库内容)</font>
        3. **<font style="color:rgb(64, 64, 64);">Visibility:</font>**<font style="color:rgb(64, 64, 64);"> </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">Public</font>**`
    3. **<font style="color:rgb(64, 64, 64);">Initialize this repository with:</font>**
    4. **<font style="color:rgb(64, 64, 64);">☑️</font>****<font style="color:rgb(64, 64, 64);"> Add a README file:</font>**<font style="color:rgb(64, 64, 64);"> </font>**<font style="color:rgb(64, 64, 64);">强烈勾选！</font>**<font style="color:rgb(64, 64, 64);"> </font><font style="color:rgb(64, 64, 64);">自动创建</font><font style="color:rgb(64, 64, 64);"> </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">README.md</font>**`<font style="color:rgb(64, 64, 64);"> </font><font style="color:rgb(64, 64, 64);">文件作为仓库首页介绍。</font>
    5. **<font style="color:rgb(64, 64, 64);">☑️</font>****<font style="color:rgb(64, 64, 64);"> Add .gitignore:</font>**<font style="color:rgb(64, 64, 64);"> 可选。如果勾选，选择模板 </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">Node</font>**`<font style="color:rgb(64, 64, 64);"> (适用于Three.js项目，会忽略 </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">node_modules</font>**`<font style="color:rgb(64, 64, 64);"> 等目录)。</font>
    6. **<font style="color:rgb(64, 64, 64);">☑️</font>****<font style="color:rgb(64, 64, 64);"> Choose a license:</font>**<font style="color:rgb(64, 64, 64);"> 可选。如果想声明版权，可选 </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">MIT License</font>**`<font style="color:rgb(64, 64, 64);"> (比较宽松的开源协议)。</font>
3. **<font style="color:rgb(64, 64, 64);">创建仓库：</font>**<font style="color:rgb(64, 64, 64);"> 点击绿色的 </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">Create repository</font>**`<font style="color:rgb(64, 64, 64);"> 按钮。</font>
4. <font style="color:rgb(64, 64, 64);">✅</font><font style="color:rgb(64, 64, 64);"> 此时仓库初始结构：</font>

```plain
my-threejs-journey (仓库根目录)
├── .gitignore
├── LICENSE
└── README.md
```

<h2 id="d69f83ed"><font style="color:rgb(64, 64, 64);">二、GitHub Pages 配置（核心步骤）</font></h2>
1. <font style="color:rgb(64, 64, 64);">克隆仓库到本地：</font>

```plain
git clone https://github.com/molunanli/my-threejs-journey.git
cd my-threejs-journey
```

2. <font style="color:rgb(64, 64, 64);">创建第一个 Demo 文件夹：</font>

```plain
mkdir demos\01-rotating-cube
```

3. <font style="color:rgb(64, 64, 64);">在 </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">demos/01-rotating-cube</font>**`<font style="color:rgb(64, 64, 64);"> 中放入 Three.js 文件：</font>

```plain
demos\01-rotating-cube
├── index.html
├── main.js
└── style.css (可选)
```

4. 推送代码到main分支

```plain
git add .
git commit -m "添加第一个旋转立方体demo"
git push origin mainchuang
```

5. 创建gh-pages分支

```plain
# 创建全新空白分支
git checkout --orphan gh-pages

# 删除所有文件（保留.git）
git rm -rf .

# 创建demo目录结构
mkdir demos\01-rotating-cube

# 从main分支复制demo文件
git checkout main -- demos/01-rotating-cube
```

6. 添加导航页

```plain
<!DOCTYPE html>
<html>
<body>
  <h1>我的Three.js之旅</h1>
  <ul>
    <li><a href="demos/01-rotating-cube/">01 - 旋转立方体</a></li>
  </ul>
</body>
</html>
```

7. 提交gh-pages分支

```plain
git add .
git commit -m "初始化gh-pages分支"
git push origin gh-pages
```

<font style="color:rgb(64, 64, 64);">✅</font><font style="color:rgb(64, 64, 64);"> 此时 gh-pages 分支结构：</font>

```plain
my-threejs-journey/ (gh-pages分支根目录)
├── index.html       # 导航首页
└── demos/
    └── 01-rotating-cube/
        ├── index.html
        ├── main.js
        └── style.css
```

8. 访问仓库<font style="color:rgb(64, 64, 64);">Settings → Pages</font>
9. <font style="color:rgb(64, 64, 64);">配置</font>
+ **<font style="color:rgb(64, 64, 64);">Branch</font>**<font style="color:rgb(64, 64, 64);">:</font><font style="color:rgb(64, 64, 64);"> </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">gh-pages</font>**`
+ **<font style="color:rgb(64, 64, 64);">Folder</font>**<font style="color:rgb(64, 64, 64);">:</font><font style="color:rgb(64, 64, 64);"> </font>`**<font style="color:rgb(64, 64, 64);background-color:rgb(236, 236, 236);">/ (root)</font>**`
+ <font style="color:rgb(64, 64, 64);">点击 Save</font>
+ <font style="color:rgb(64, 64, 64);">等待1~2分钟出现</font>

```plain
Your site is published at https://你的用户名.github.io/my-threejs-journey/
```

![](https://cdn.nlark.com/yuque/0/2025/png/42866959/1751704834324-429ec758-0473-45a1-96cb-b3ae7fbb518b.png)

10. 此时可以访问页面

![](https://cdn.nlark.com/yuque/0/2025/png/42866959/1751704901952-d1be7304-2103-408e-acb3-3b3b105d6b71.png)

