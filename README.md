# Notes-1806008
{\bf Day 4:}
in assigns something within the x\\
x= [1,2,3]\\
print(1 in x)\\
\textit{Returns true because one is in x}\\
\textit{This is useful so that we can determine if something within the set that you are testing.}
\begin{itemize}
\item lists\\
indexing the list is always starting with zero.
\textit{Examples\\}
indexing\\
\hspace*{.2in}x=[1,2,3]\\
\hspace*{.4in}print(x[1])\\
\textit{Result is the first second element in the set.}

\hspace*{-.2in}\underline{2D array}\\
\hspace*{.2in}x=[[1,2],[3,4]]\\
\hspace*{.4in}print(x[0][1])\\
\textit{Result from the print would print 2}\\

\hspace*{.2in}x=[[1,2],[3,4]]\\
\hspace*{.4in}print(x[1][1])\\
\textit{Result from the print would print 4}\\

\hspace*{.2in}x=[[1,2],[3,4]]\\
\hspace*{.4in}print(x[0][1], end = ", ")\\
\textit{Result from the print would print 2}\\
\textit{Note that the 'end = ","' replaces the new line command in python and instead uses the comma... this is useful when printing multiple results that are needed to be used in an array vs separte results}\\
\item nested for loop\\
\hspace*{.2in}x=[[1,2,3],[4,5,6],[7,8,9]]\\
\hspace*{.2in}for i in range(len(x)):\\
\hspace*{.4in}for j in range(len(x[i])):\\
\hspace*{.6in}print(x[i][j])\\
\textit{Results in matrix}\\
Writing Matrix multiplication of a scalar and array\\
\hspace*{.2in}x=[[1,2,3],[4,5,6],[7,8,9]]\\
\hspace*{.2in}for i in range(len(x)):\\
\hspace*{.4in}for j in range(len(x[i])):\\
\hspace*{.6in}print(2*x[i][j])\\
\textit{Results in matrix items multiplied by 2\\ to set up as a matrix change it to:\\}

\hspace*{.2in}x=[[1,2,3],[4,5,6],[7,8,9]]\\
\hspace*{.2in}newx = [ ]\\
\hspace*{.2in}for i in range(len(x)):\\
\hspace*{.4in}rowx = [ ]\\
\hspace*{.4in}for j in range(len(x[i])):\\
\hspace*{.6in}rowx.append(2*x[i][j])\\
\hspace*{.4in}print(rowx)\\
\hspace*{.4in}newx.append(rowx)\\
\hspace*{.2in}print(newx)\\
\textit{Results in matrix items multiplied by 2}\\ 
$$i = \left(\begin{array}{ccc}
2,4,6 \\
8,10,12 \\
14,16,18
\\
\end{array}\right)$$
\textit{This sets it up as a matrix vs sending it to the independent results:\\ The row.append$\dots$ just says after each item is done in the perenthesis, then is sent to the variable labled before the period. So after each for loop the append takes whats in the parenthesis and then spits it into the variable labled outside the list.\\}
\item Function definition\\
\hspace*{.2in}def f(x,y)\\
\hspace*{.4in}result = x*y\\
\hspace*{.2in} f(2,3)\\
\textit{Results in $6$\\}
\newpage
\item Doc Strings\\
""" """\\
These quotes describe the function and are needed on all homeworks.\\
Example:\\
vectormult(x,a):\\
""" """\\
b=[]\\
for i in range(len(x)):\\
b.append(x[i]*a)\\
return b\\
x=[1,2,3]\\
a = 2\\
result=vectormult(x,a)\\
print(result)\\

def valuesofmatrix(x):
  s=[]
  for i in range(len(x)):
    for j in range(len(x[i])):
      s.append(x[i][j])
  return s

x=[[1,2,3],[4,5,6],[7,8,9]]
result=valuesofmatrix(x) 
#print(result)
for k in range(len(result)):
  print(result[k])
