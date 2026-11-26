# Context-Aware Restaurant Recommendation with Taichung Bus Accessibility

結合台中公車可及性的情境感知餐廳推薦（IEEE 會議論文格式的研究提案）


## 連結

- **Overleaf project:** https://www.overleaf.com/project/6b0781e7368cb989823c3c2b/share#c50db28c19a230a1c35d229b49128d49530a7c420696cf2b
- **PDF:** [`ieee_latex/DIC_4.pdf`](ieee_latex/DIC_4.pdf)

## 專案結構

```
ieee_paper.tex        
bib/ieee_paper.bib    
ieee_latex/DIC_4.pdf
```

## 編譯方式

### Overleaf

1. 上傳 `ieee_paper.tex` 與 `bib/` 資料夾，保留目錄結構。
2. 在 Menu → Compiler 選擇 **pdfLaTeX**。
3. 按 **Recompile**。

### 本機（TeX Live 或 MiKTeX）

```bash
latexmk -pdf ieee_paper.tex
```

或手動執行：

```bash
pdflatex ieee_paper
bibtex ieee_paper
pdflatex ieee_paper
pdflatex ieee_paper
```

中文作者名使用 `CJKutf8` 套件與 `bkai` 字型，本機需安裝 CJK 及 Arphic 字型套件。

主要套件：`IEEEtran`、`cite`、`CJKutf8`、`amsmath`、`booktabs`、`tabularx`、`algorithm`、`algpseudocode`、`tikz`。
