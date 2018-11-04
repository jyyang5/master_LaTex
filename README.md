# master_Latex
## Contents

- Insert figure 

- Insert table 

- Math equations

### Insert figure 
- Centred (figure*)
- Figure name(\caption{})

```
\begin{center}
\begin{figure*}
\includegraphics[height=2.2in, width=5.4in]{figureName}
\caption{Opt. expected fitness gain and corsponding opt. normalized step size of the surrogate model assisted $(\mu/\mu,\lambda)$-ES plotted against the noise-to-signal ratio. The line and dots with colour black, blue green represent $(3/3,10)$-ES, $(3/3,10)$-ES, $(3/3,10)$-ES The solid line representa the results obtained analytically when $n\rightarrow \infty$. }
\end{figure*}
\end{center}
```

### Insert table 
- Centred (Ttable*)
- Table name (\caption{})
- Put an extra line to sperate content (\toprule)
- Reference(\label{Tab:Test_result} **after** \end{tabular})

```
\begin{table*} 
\caption{Median test results.}
\begin{tabular}{ l *{5}{D{.}{.}{4}} }
\toprule
\textbf{} & \multicolumn{5}{c}{\textbf{Median number of objective function calls (with model assistance) }} \\
\cmidrule(lr){2-6}
\textbf{Test functions} & \multicolumn{1}{c}{$(1+1)$-ES} & \multicolumn{1}{c}{$(3/3,10)$-ES} & \multicolumn{1}{c}{$(5/5,20)$-ES} & \multicolumn{1}{c}{$(10/10,40)$-ES}  \\
\midrule
\texttt{linear sphere} &1.72\% &4.65\% &9.84\% &19.17\%      \\
\texttt{quadratic sphere} &3.00\% &8.39\% &18.31\%  &28.09\% \\ 
\texttt{cubic sphere} &4.13\% &8.64\% &14.51\% &25.83\%      \\ 
\texttt{Schwefel\' s function} &7.78\% &18.28\% &31.58\% &64.43\%\\ 
\texttt{quartic function} &2.21\% &7.37\% &15.55\% &32.48\%    \\ 
        \bottomrule             
\end{tabular}
\label{Tab:Test_result}
\end{table*}
```


### Math equations
- Get reference 
- Centered
- Numbered 
- Aligned 

```{tex}
\begin{align}
\Delta &= -\frac{N}{2} E \left [  \log f(y) - \log {f(x)} \right ] \nonumber\\
 &= -\frac{N}{2} E \left [  \log \frac{f(x^{t+1})}{f(x^{t})} \right ], 
\end{align}
```
