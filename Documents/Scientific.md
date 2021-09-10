# 软件推荐 1 - 学术科研类

平常在学习工作或者科研实验的时候，经常会遇到软件不知道怎么选的问题，尤其是当有标准化的需求，比如文字排版、图表制作等，或者想要降低试错成本。本文将非常主观地结合一些个人使用经验帮助可能有需要的同学找到合适的软件和工具。

---

## Markdown

<div>
	<center>
	<img src="https://cdn.jsdelivr.net/gh/Nikucyan/Share/Images/1_MD.png"
    	alt="Markdown" 
    	style="zoom:28%;" />
    </br>
    Markdown Logo
</div>

### 简介

很多人想到起草文稿或者记笔记肯定会先想到 Microsoft Office 系列的 Word、One Note、记事本等，但是 Word 实际是属于相对正式的排版软件而非码字软件，会让人觉得有些不顺手也很正常（各种很血压的情况大家也应该遇到不少）；而用系统自带的记事本或写字板，功能不齐全，插图打代码什么的也不方便；Notability 好用是真好用，但也不是所有人都能有 iPad（也不是所有人能能喜欢在 iPad 上手写），如果是纯 PC 党或者需要带代码高亮等情况就很不适合。

在此，隆重推荐最适合码字的工具：**Markdown**

MarkDown 属于轻量级的标记语言，通过纯文本格式编写并生成可实时预览的 XHTML 文档，而且对图片、表格、公式、超链接、代码高亮皆有支持（部分功能不是所有编辑器都有）。目前很多网站和论坛也支持使用 Markdown 编辑，如 GitHub、CSDN、简书、Reddit 等。大部分编辑器也都是免费甚至是开源的，对学生而言十分友好。另外其语法十分简单，如用 `#` 和多个 `#` 表示不同大纲等级的标题；用 `-` 表示无序列表，用 `* ... *` 和 `** ... **` 表示斜体和粗体，用 `![图片标题](超链接)` 引用图片（部分编辑器还支持本地图片引用）等，上手极快。

### 推荐软件

1. **Typora**（本文档都是用 Typora 进行编写）

   ![Typora](https://cdn.jsdelivr.net/gh/Nikucyan/Share/Images/1_Typora.png)

   >  **推荐指数：10/10**

   Typora 是目前少数可实时像 Word 一样预览内容的 Markdown 的编辑器（实际上是网页浏览器，可以使用 `shift + F12` 调出控制台）
   
   - 优点：无需登录，支持多平台，界面很简洁美观，所见即所得，支持自定义主题（有 GitHub 主题页面），可以直接看大纲目录，也支持很多 Word 系快捷键，支持绝大部分 HTML / CSS 标签，支持自动保存，支持 LaTeX​ 公式和公式块，支持本地图片复制粘贴，如果配合 PicGo + GitHub 之类作为图床还可以实现图片自动上传并添加 URL 链接甚至是 CDN 加速访问，支持智能标点，支持 PDF、LaTeX、Word、网页等多种格式导出；
   - 缺点：不是传统 Markdown 编辑器，如果喜欢传统的分屏用代码控制 + 实时预览的话会不太合适，非开源，可能有少量 bug（比如在写这篇文章的时候自动保存失效了一次，怨念）；
   - 适合人群：频繁使用电脑做笔记、写草稿等需要快速记录的工作而且可能需要打公式和代码块的人。
   
   <div>
   	<center>
   	<img src="https://cdn.jsdelivr.net/gh/Nikucyan/Share/Images/1_Typora_Screen.png"
       	alt="Typora Screenshot" 
       	style="zoom:60%;" />
       </br>
       Typora 的用户界面
   </div>

2. **作业部落 Cmd Markdown**

   ![CMD Logo](https://www.zybuluo.com/static/img/logo.png)

   > **推荐指数：8/10**

   - 优点：有网页版，甚至可以不下载在线使用，支持多平台，支持自动云端保存（需登录），支持把自己的文稿发布于作业部落官方提供的平台，支持 LaTeX 公式和公式块，支持高效绘制流程图（用代码），有可视化操作按钮；
   - 缺点：大部分功能需要注册登录，一些功能（如上传图片、导出完整 PDF 和网页等）还需要会员，对生态锁得比较死，编辑器偶尔会出现显示错误的 bug，非开源；
   - 适合人群：同上，同时有便捷分享和作图床使用的需求。

   <div>
   	<center>
   	<img src="https://cdn.jsdelivr.net/gh/Nikucyan/Share/Images/1_CMD_Screen.png"
       	alt="CMD Screenshot" 
       	style="zoom:60%;" />
       </br>
       作业部落 CMD Markdown 的用户界面
   </div>

### 联动软件推荐

1. **PicGo**

   上面已经提到了，需要在类似 GitHub 一类提供文件 / 代码托管服务的平台上建立仓库，PicGo 会使用 Token 的形式得到上传许可并提交更新到远程仓库。只需要简单的配置也可以实现使用第三方 CDN 加速（比如我使用的是免费开源的公共 CDN：jsDelivr，相对应的图片网址就改为 `https://cdn.jsdelivr.net/gh/[directory_in_GH_Repo]`），这样在 Typora 中开启 PicGo 的联动功能就可以把复制进去的图片一口气上传到自己的对应仓库并更改引用链接为经过加速的链接。



## $\mathrm{\LaTeX}$​

### 简介

上面说到 Word 属于排版工具，那科研排版能用 Word ……吗？

> Word：你再骂？

答案也是不行的（Word 就是废物啊）。Word 在公式编辑方面极不规范，极易导致公式在复制粘贴或者格式转换后就无法使用，加上还有行间使用的表示数学符号的如 $\phi$​​​​ 之类都会出现错误显示的情况（变成 UTF-8 / Unicode 字符），还有规范引用文献的问题，即使现在一些教授可以接收 Word 编辑的实验报告和作业，以后需要正式地发表到一些出版平台（尤其是国外期刊的出版商，比如 Elsevier、IEEE、Springer、Wiley 等）大多需要使用规定的 **LaTeX** 模板进行排版，而且很可能完全不接受 Word 文档。这个时候学习使用 LaTeX 就很有必要。

<div>
	<center>
	<img src="https://cdn.jsdelivr.net/gh/Nikucyan/Share/Images/1_LaTeX.svg"
    	alt="LaTeX" 
    	style="zoom:70%;" />
    </br>
    The LaTeX Project
</div>

LaTeX 是一种文字编辑的标准，是 TeX 标准上的扩展。编辑需要全程使用代码（有少数所见即所得式编辑器，但是我没试过就不推荐了）。通常 LaTeX 需要先声明使用的文章类别（`\documentclass{}`）和宏包（`\usepackage{}`），类似于在 C 语言中声明运行库（`#include<stdio>`）和定义函数（`#define [some function]`）的作用。其最大特点在于在文章中通过 `$ ... $` 或 `$$ ... $$` 在行中 / 行间表示数学环境（更正式可以使用 `\begin{equation} ... \end{equation}` 表示），如广义薛定谔方程：`$$\hat{H} \Psi = i \hbar \frac{\partial}{\partial t} \Psi$$` 即为 
$$
\hat{H} \Psi=i \hbar \frac{\partial}{\partial t} \Psi​
$$
，也可以很方便建立矩阵等；其次可以使用 `\ref{}` 和 `\label{}` 的标签做到很便捷的引用功能；文章的各个部分也可以分别在不同文件中写完，最后再使用主文章包含进去；参考文献也有专门的管理文件系统。另外对于化学类学生，LaTeX 同时支持简单的化学式表达和有机物绘制，如 `\ce{CH3COOH}` 即为 $\ce{CH3COOH}$（需要使用 `mhchem` 宏包）​​​。

但说句实话，LaTeX 属于易学难精，日积月累才能灵活运用。即使 LaTeX 不是最方便的工具，它却是最符合科技文章规范的，而且在引用和公式这两点上 Word 反正是望尘莫及。我用 LaTeX 写各种报告和作业已经 3 年有余，现在也尝试使用 LaTeX 制作简历、幻灯片等材料，观感上还是很不错的。

### 推荐软件

1. **WinEdt**

   ![WinEdt Logo](https://cdn.jsdelivr.net/gh/Nikucyan/Share/Images/1_WinEdt.png)

   > **推荐指数：7/10** （非 CTEX 版本：4/10）

   如果对中文有需求推荐直接使用（基于 WinEdt 编辑器的）CTeX，对中文有较好支持。

   - 优点：功能完善，基本上作为 LaTeX 编辑器需要的功能他都有提供，支持大量 TeX 系列程序，支持拼写检查，有希腊字母和数学符号等的 GUI 菜单，很适合新人入门，支持多标签页，支持；
   - 缺点：也太难用了吧，简直是〇〇，且不提本身是非免费不开源的商业软件，每次写完都得手动点编译（如果是使用非原生字体还需要调用 XeLaTeX 程序，不能够使用快捷键），本身不整合 PDF 预览器（通常是要外部调用 SumatraPDF），只支持 Windows，还好像没中文……；
   - 适合人群：从入门到入土。

2. **Overleaf**

   <img src="https://cdn.jsdelivr.net/gh/Nikucyan/Share/Images/1_Overleaf.png" alt="Overleaf Logo" style="zoom:40%;" />

   > **推荐指数：7/10**

   我可不信你在谷歌搜 LaTeX 会没见过这玩意……

   - 优点：多人合作（别问我体验如何，笑死我周围根本没人用 LaTeX），在线编辑，支持自动保存，相对美观的 UI，有大量模板可以使用，便捷的项目管理，支持代码自动补完，支持非严谨语法（比如不在数学环境中调用部分数学公式）；
   - 缺点：非严谨语法但很可能不能被其他软件识别，也不适合新手入门学习语法，没有常用字符菜单；
   - 适合人群：过了萌新期，以及需要合作编辑的人。

3. **Visual Studio Code**

   <img src="https://cdn.jsdelivr.net/gh/Nikucyan/Share/Images/1_VSC.png" alt="VSCode Logo" style="zoom:32%;" />

   > **推荐指数：4/10**

   - 优点：VSCode 有什么优点就有什么优点（搁这搁这呢），开源；
   - 缺点：无内置预览器等，需要手动配置环境和 SumatraPDF 之类的预览器，对新手来说不友好；
   - 适合人群：已经熟悉掌握了 LaTeX 语法和有一定手动配置环境等基础的人。

### 联动软件推荐

1. **Mathpix Snipping Tool**

   遇到了 PDF 或者图像里（甚至是手写）的公式没办法复制自己打又太麻烦？那就应该试试这个神器了。Mathpix Snipping Tool 提供了对数学公式优化得最好的 OCR，只需要截图（或者用手机端拍照）就可以显示出来正确的 LaTeX 公式，识别率不低但是毕竟 OCR 还是做不到 100%，反正可以极大方便新手和懒人（我），而且最好的是还支持 Word 的公式格式，即使不是 LaTeX 党也可以轻松使用。

2. **gnuplot**

   不是，不会这年头还有人用 gnuplot 吧，不会吧不会吧（x

   gnuplot 是一个 Linux 平台的命令行交互式绘图工具（当然也可以在 Windows 上使用，是基于 Cygwin 虚拟机的移植），虽然很难用但是碍于能和 LaTeX 联动使用就不骂他了，而且可以使用线性插值平滑图像（你 MATLAB 做得到吗？.jpg）。使用 gnuplot 作图结束之后可以使用 

   ``` Bash
   set terminal epslatex 
   set output '[Filename].tex'
   plot "[DataFile].dat"
   set output
   ```

   命令来实现导出供 LaTeX 导出的 `.tex` 文件和相同文件名的 `.eps` 文件。在 LaTeX 中使用 `\input{[Filename].tex}` 即可将矢量图像导入到文档中（推荐加上 `\begin{figure} ... \end{figure}` 的指令，以插入图形的形式更好地规定一些其他参数）。
   
3. **Excel**

   即使是使用了很长时间的人也经常会有 LaTeX 做表格很不方便的感觉，那能不能把 Excel 表格导入到 LaTeX 呢，这里就需要用到一个插件：**Excel2LaTeX**

   安装完成之后，需要手动在 `File - Options - Add-ins - Manage` 中手动启用，此后就会显示在最上方工具栏的 `Add-ins`，在 Excel 中选择合适的表格区域再打开这个插件 `Convert table to LaTeX` 按钮就可以调整各种参数和导出所需的 LaTeX 版本的表格了，对应的表格线也会被一并加入。注意可能会需要用到一些其他的宏包以避免报错。

   
