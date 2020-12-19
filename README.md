#+title: Operating Systems - Lab 2
#+author: Qinyang Wu (3519174) @@latex:\\@@ Zamik Shahid(3507157) @@latex:\\@@ Tilak Wälde (2662598)
#+options: toc:nil num:nil
#+latex_header: \usepackage{fullpage}
#+latex_header: \usepackage{parskip}
#+latex_header: \usepackage{multicol}
#+LATEX_HEADER: \usepackage{tikz}
#+LATEX_HEADER: \usepackage{minted}
#+LATEX_HEADER: \usetikzlibrary{tikzmark}
#+LATEX_HEADER: \usepackage{makecell}
#+latex_header: \usepackage{listings}
#+latex_header: \usepackage{tcolorbox}
#+latex_header: \usepackage{fontspec,xltxtra,xunicode}
#+latex_header: \setmonofont[Scale=MatchLowercase]{Hack}

* Exercise 1
** a - list all child processes of =PID 1=
According to the manpage of =ps= we can use the following options:

#+ATTR_LATEX: :options frame=single
#+BEGIN_SRC text
   a      Lift the BSD-style "only yourself" restriction, which is imposed upon the
          set of all processes when some BSD-style (without "-") options are used or
          when the ps personality setting is BSD-like.  The set of processes selected
          in this manner is in addition to the set of processes selected by other
          means.  An alternate description is that this option causes ps to list all
          processes with a terminal (tty), or to list all processes when used together
          with the x option.

   u      Display user-oriented format.

   --ppid pidlist
          Select by parent process ID.  This selects the processes with a parent
          process ID in pidlist.  That is, it selects processes that are children of
          those listed in pidlist.
#+END_SRC

