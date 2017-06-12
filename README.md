# Contributing

## Formatting

### Section Numbering
Not every section of Mendelson has exercises.
To start numbering sections at `n`, set the section counter to `n-1` before the `\section` comand:

```latex
\setcounter{section}{n-1}
\section{The Nth Section Name}
```

### Problems

There is a `problem` environment defined in `topology.tex`.
Problems are automatically numbered by default, but you can set what problem number by hand if you're skipping some problems.

Examples:

Using automatic numbering:
```latex
\begin{problem}
Show that $x^2 = x*x$.
\end{problem}
```

Manually numbering:
```latex
\begin{problem}[5]
Show that $x \in X$.
\end{problem}

\begin{problem} % Will automatically be numbered as problem 6
Show that $y \in Y$.
\end{problem}
```

### Proofs

Please use the `proof` environment.
It is borrowed from `amsthm` but tweaked to include a line break after the proof name.
We strongly recommend stating what it is you are proving, especially in problems with multiple parts or claims.

When doing a proof by contradiction, you may use the `\contradiction` command to draw two arrows (`-><-`) indicating a contradiction.
You may use the command in either math mode or text mode.

## Authors
Make sure to add your name to the authors list in `topology.tex`!
