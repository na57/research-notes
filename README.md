# 研究工作笔记

## 内容
- 阅读笔记
    - [Botnet](paper-reviews/botnet.pdf)
    - [CNN](paper-reviews/cnn.pdf)
    - [机器学习](paper-reviews/machine-learing.pdf)
    - [大米分级](paper-reviews/rice-grading.pdf)
- 其他
    - [思政课作业](other/zz.pdf)
    - [论文阅读作业](other/cyclegan.pdf)

    
## LaTex 代码段

### 插入图片

引入相关宏包：
```latex
\usepackage{graphicx} %插入图片的宏包
\usepackage{float} %设置图片浮动位置的宏包
\usepackage{subfigure} %插入多图时用子图显示的宏包
```

代码：
```latex
\begin{figure}[H]
	\centering
	\includegraphics[width=0.7\textwidth]{path}
	\caption{}
	\label{}
\end{figure}
```

相关说明：
- `\begin{figure}[H]` H 为当前位置
- `\centering` 图片居中
- `\includegraphics[width=0.7\textwidth]{path}`  插入图片，[]中设置图片大小，{}中是图片文件名
- `\caption{}`  最终文档中希望显示的图片标题
- `\label{Fig.main2}` 用于文内引用的标签


### 多行公式一个编号，且对齐

代码：
```latex
\begin{equation}
  \begin{split}
  	optimize F \\
	s.t. \ D &\leq D_0 \\
	L &\leq L_0
  \end{split}
\end{equation}
```