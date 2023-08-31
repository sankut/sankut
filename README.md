\documentclass{article}
\usepackage{tikz}
\usepackage{pgfplots}

\begin{document}

\begin{figure}
\centering
\begin{tikzpicture}
    \begin{axis}[
        ybar stacked,
        bar width=30pt,
        ymin=0,
        ymax=100,
        ylabel={Percentage},
        xtick=data,
        xticklabels={Exercise Area, Circulation Space, Anthropometry},
        legend style={at={(0.5,-0.15)},
          anchor=north,legend columns=-1},
    ]
    \addplot[fill=blue] coordinates {(0,70)};
    \addplot[fill=green] coordinates {(0,50)};
    \addplot[fill=red] coordinates {(0,20)};
    \legend{Upper Limit, Lower Limit, Actual Allocation}
    \end{axis}
\end{tikzpicture}
\caption{Space Allocation in the Gym}
\end{figure}

\end{document}

