Add space between columns in a table.
```tex
\setlength{\tabcolsep}{12pt}
```

Resize table to fit width.
```tex
% Please add the following required packages to your document preamble:
% \usepackage{multirow}
% \usepackage{graphicx}
\begin{table}[]
\centering
\caption{}
\label{tab:my-table}
\resizebox{\textwidth}{!}{%
\begin{tabular}{llllll}
Structure & Area & \multicolumn{4}{c}{Weighing factors} \\
 &  & 1 & 2 & 5 & 10 \\
\multirow{2}{*}{Arteries} & Full ROI & \textbf{81.97+-0.22} & 81.25+-0.31 & 80.97+-0.29 & 79.88+-1.71 \\
 & Small Vessels & 78.67+-0.41 & 78.23+-0.39 & 79.52+-0.59 & \textbf{80.00+-0.33} \\
\multirow{2}{*}{Veins} & Full ROI & \textbf{87.16+-0.24} & 86.77+-0.08 & 86.28+-0.26 & 85.10+-1.39 \\
 & Small Vessels & 80.03+-0.57 & 80.28+-1.07 & 81.33+-0.20 & \textbf{81.39+-1.12}
\end{tabular}%
}
\end{table}
```

Table cell with multiple lines.
```tex
\documentclass{article}
\begin{document}
\begin{tabular}{cccc}
  One & Two & Three & Four \\
  Een & Twee & Drie & Vier \\
  One & Two & 
    \begin{tabular}{@{}c@{}}Three \\ Drie\end{tabular}
  & Four
\end{tabular}
\end{document}
```
