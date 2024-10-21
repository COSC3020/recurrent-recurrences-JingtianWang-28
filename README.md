# Recurrent Recurrences

Give big $\Theta$ bounds for the following recurrence relations.

1.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        T\left(\frac{n}{13}\right) + 5 & n > 1
    \end{cases}
$$

2.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        13 T\left(\frac{n}{13}\right) + 5 & n > 1
    \end{cases}
$$

3.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        13 T\left(\frac{n}{13}\right) + 2n & n > 1
    \end{cases}
$$

///
$T(n/13) = T(n/169)+5$\
$T(n) = T(n/169)+5+5...$\
$T(n) = T(n/13^3)+5+5+5...$\
$T(n) = T(n/13i)+5i$\

$for i = log(n) = T(1) + 5log(n)$\
$5log(n) ∈ theta log(n)$\
T(n) exist in theta log(n)\

2)
$T(n) = 13T(n/13)+5$\
$T(n/13) = 13T(n/169)+5$\
$T(n) = 13(13T(n/169)+5)+5 = 169T(n/169)+13*5+5$\
$T(n) = 169T(n/169)+65+5$\
$T(n) = 13^3(T)(n/13^3)+65+65+5...$\
$T(n) = (13^i)T(n/13^i)+5i$\

$i = log_13(n)$\
$T(n) = (13^log_13(n))T(1)+5log_13(n)$\
$T(n) = nT(1)+5log_13(n)$\
$T(n) ∈ theta (n)$\

4)
$T(n) = 13T(n/13)+2n$\
$T(n/13) = 13T(n/169)+2(n/13)$\
$T(n) = 13(13T(n/169)+2(n/13))+2n = 169T(n/169)+26(n/13)+2n$\
$T(n) = 169T(n/169)+2n+2n...$\
$T(n) = 13^i(T)(n/13^i)+2ni$\

$i = log_13(n)$\
$T(n) = nT(1)+2nlog_13(n)$\
$T(n)∈theta(nlogn)$\


###
https://web.stanford.edu/class/archive/cs/cs161/cs161.1168/lecture3.pdf
Sources: chatgept provide me with ideas for proof methods. And complete the assignment through the examples and theorems on the above website.

Plagiarism Statement: “I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.”
