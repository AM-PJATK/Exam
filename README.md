# Exam

\documentclass{article}
\usepackage{amsmath}
\usepackage{amssymb}

\begin{document}

\section{The Limit of a Function}

\subsection*{Definition (by Heine)}
Suppose \( x_0 \in \mathbb{R} \cup \{-\infty, +\infty\} \). Let \( f \) be a function defined on a contiguity \( S(x_0) \) of a point \( x_0 \). We say that \( g \in \mathbb{R} \cup \{-\infty, +\infty\} \) is \textit{the limit of the function} \( f \) \textit{at the point} \( x_0 \), provided that:

for every sequence \( (x_n) \) of elements of the contiguity \( S(x_0) \), with limit \( x_0 \),

\( g \) is the limit of a sequence \( (f(x_n)) \).

The fact that \( g \) is the limit of a function \( f \) at the point \( x_0 \) is denoted as

\[
\lim_{x \to x_0} f(x) = g \quad \text{or} \quad f(x) \underset{x \to x_0}{\longrightarrow} g.
\]

\noindent For \( g \in \mathbb{R} \), the limit is called the finite limit. For \( g \in \{-\infty, +\infty\} \), we say that the limit is infinite.

It can be shown that if the limit (or one-sided limit) of a function at a point exists then it is unique, i.e., it is not possible that a function has two different limits at a point.

The last definition implies a very useful corollary.

\subsection*{Corollary}
If in \( S(x_0) \) there exist two sequences \( (a_n) \), \( (b_n) \), both with the limit \( x_0 \), and the limits of sequences \( (f(a_n)) \), \( (f(b_n)) \) are different, then the limit of the function \( f \) at the point \( x_0 \) does not exist.

\subsection*{Example}
Using the last corollary we will prove that the limit of the function \( y = \sin(1/x) \) at the point \( x_0 = 0 \) does not exist. Consider the sequences with general terms

\[
a_n = \frac{1}{2\pi n + \frac{\pi}{2}}, \quad b_n = \frac{1}{2\pi n}.
\]

Obviously, both have the limit 0, but the sequence \( \left( \sin\left( \frac{1}{a_n} \right) \right) \) has the limit 1, whereas the sequence \( \left( \sin\left( \frac{1}{b_n} \right) \right) \) has the limit 0.


\section{The Limit of a Function}

\subsection*{Theorem}
The following limits should be remembered:

\begin{enumerate}
    \item \[
    \lim_{x \to 0} \frac{\sin x}{x} = 1
    \]

    \item \[
    \lim_{x \to 0} (1 + x)^{\frac{1}{x}} = e, \quad \lim_{x \to \infty} \left( 1 + \frac{1}{x} \right)^x = e, \quad \lim_{x \to -\infty} \left( 1 + \frac{1}{x} \right)^x = e
    \]

    \item \[
    \lim_{x \to \infty} a^x = 
    \begin{cases} 
    \infty & \text{for } a > 1 \\
    0 & \text{for } a \in (0,1)
    \end{cases}, \quad 
    \lim_{x \to -\infty} a^x = 
    \begin{cases} 
    0 & \text{for } a > 1 \\
    \infty & \text{for } a \in (0,1)
    \end{cases}
    \]

    \item \[
    \lim_{x \to 0} x^{-\alpha} = \infty \quad \text{for } \alpha > 0, \quad \lim_{x \to \infty} x^{-\alpha} = 0 \quad \text{for } \alpha > 0
    \]

    \item \[
    \lim_{x \to -\infty} \arctan x = -\frac{\pi}{2}, \quad \lim_{x \to \infty} \arctan x = \frac{\pi}{2}, \quad \lim_{x \to \infty} \text{arccot } x = \frac{\pi}{2}, \quad \lim_{x \to -\infty} \text{arccot } x = 0
    \]

    \item \[
    \lim_{x \to \infty} \ln x = \infty, \quad \lim_{x \to 0^+} \ln x = -\infty
    \]

    \item \[
    \text{if } w_m(x) = a_m x^m + a_{m-1} x^{m-1} + \dots + a_1 x + a_0, \quad w_n(x) = b_n x^n + b_{n-1} x^{n-1} + \dots + b_1 x + b_0,
    \]
    \[
    \text{where } a_m \neq 0, \, b_n \neq 0, \text{ then}
    \]
    \[
    \lim_{x \to \infty} \frac{w_m(x)}{w_n(x)} = 
    \begin{cases}
    0 & \text{for } m < n \\
    \frac{a_m}{b_n} & \text{for } m = n \\
    \text{sgn} \left( \frac{a_m}{b_n} \right) \infty & \text{for } m > n
    \end{cases}
    \]
\end{enumerate}

The limits \(\lim_{x \to \infty} w_m(x)\) and \(\lim_{x \to \infty} \frac{w_m(x)}{w_n(x)}\) can be determined by the use of the formula:

\[
\lim_{x \to \infty} f(x) = \lim_{x \to -\infty} f(-x).
\]
\subsection*{Example}


    $\displaystyle \lim_{x \to 1} \frac{2x+4}{x-2} = \frac{2+4}{1-2} = -6$
    
    $\displaystyle \lim_{x \to \infty} \frac{2x+4}{x-2} = \left| \begin{array}{c} \text{nominator and denominator are} \\ \text{polynomials of the same degree} \end{array} \right| = \frac{2}{1} \quad \text{or}$
    
    $\displaystyle \lim_{x \to \infty} \frac{2x+4}{x-2} = \lim_{x \to \infty} \frac{x(2+\frac{4}{x})}{x(1-\frac{2}{x})} = \lim_{x \to \infty} \frac{2+\frac{4}{x}}{1-\frac{2}{x}} = \frac{2+\frac{4}{\infty}}{1-\frac{2}{\infty}}$
    
    $\displaystyle \lim_{x \to \infty} \frac{x^2-4}{2x+3} = \left| \begin{array}{c} \text{nominator and denominator are} \\ \text{polynomials and degree of the} \\ \text{denominator $>$ degree of the nominator} \end{array} \right| = \operatorname{sgn}\left(\frac{1}{2}\right) \cdot \infty = \infty \quad \text{or}$
    
    $\displaystyle \lim_{x \to \infty} \frac{x^2-4}{2x+3} = \lim_{x \to \infty} \frac{x^2(1-\frac{4}{x^2})}{x(2+\frac{3}{x})} = \lim_{x \to \infty} x \cdot \lim_{x \to \infty} \frac{1-\frac{4}{x^2}}{2+\frac{3}{x}} = \infty \cdot \frac{1-\frac{4}{\infty^2}}{2+\frac{3}{\infty}} = \infty \cdot \frac{1}{2} = \infty$
    
$\displaystyle \lim_{x \to -\infty} \frac{x^2-4}{2x+3} = \lim_{x \to -\infty} \frac{(-x)^2-4}{2(-x)+3} = \lim_{x \to \infty} \frac{x^2-4}{-2x+3} = \left| \begin{array}{c} \text{nominator and denominator are} \\ \text{polynomials of the same degree} \end{array} \right| =$
    
    $= \operatorname{sgn}\left(\frac{1}{-2}\right) \cdot \infty = -\infty$
    
 $\displaystyle \lim_{x \to -3} \frac{x+3}{x^2-9} = \left[\frac{0}{0}\right] = \lim_{x \to -3} \frac{x+3}{(x-3)(x+3)} = \lim_{x \to -3} \frac{1}{x-3} = \frac{1}{-3-3} = -\frac{1}{6}$
    
$\displaystyle \lim_{x \to \infty} \frac{x+3}{x^2-9} = \left| \begin{array}{c} \text{nominator and denominator are} \\ \text{polynomials and degree of the} \\ \text{denominator $<$ degree of the nominator} \end{array} \right| = 0.$
    
$\displaystyle \lim_{x \to \infty} \frac{\sqrt{4x+1}-5}{\sqrt{x+2}-3} = \left[\frac{\infty}{\infty}\right] = \lim_{x \to \infty} \frac{\sqrt{x}\left(\sqrt{4+\frac{1}{x}}-\frac{5}{\sqrt{x}}\right)}{\sqrt{x}\left(\sqrt{1+\frac{2}{x}}-\frac{3}{\sqrt{x}}\right)} = \lim_{x \to \infty} \frac{\sqrt{4+\frac{1}{x}}-\frac{5}{\sqrt{x}}}{\sqrt{1+\frac{2}{x}}-\frac{3}{\sqrt{x}}} = \frac{\sqrt{4+\frac{1}{\infty}}-\frac{5}{\sqrt{\infty}}}{\sqrt{1+\frac{2}{\infty}}-\frac{3}{\sqrt{\infty}}} = \frac{2}{1} = 2.$
    
$\displaystyle \lim_{x \to 0} \frac{\sin 2x}{\sin 3x} = \lim_{x \to 0} \frac{\sin 2x}{2x} \cdot \frac{3x}{\sin 3x} \cdot \frac{2}{3} = \lim_{x \to 0} \frac{\sin 2x}{2x} \cdot \lim_{x \to 0} \frac{3x}{\sin 3x} \cdot \frac{2}{3} = \left|\begin{array}{c} y = 2x \quad y \to 0 \\ w = 3x \quad w \to 0 \end{array}\right| =$
    
    $= \frac{2}{3} \cdot \lim_{y \to 0} \frac{\sin y}{y} \cdot \lim_{w \to 0} \frac{w}{\sin w} = \frac{2}{3}$

\section{Newton's method}

Let's apply Newton's method to find an approximate value of the root of the given equations within the specified intervals. Newton's method is an iterative process given by the formula:

\[ x_{n+1} = x_n - \frac{f(x_n)}{f'(x_n)} \]

where \( x_n \) is the current approximation, and \( f'(x_n) \) is the derivative of the function at \( x_n \).

Part (a): \( f(x) = x^5 - x - 1 \) in the interval \([1, 2]\)

Step 1: Initial Guess and Derivative Calculation

Choose an initial guess \( x_0 \) within the interval \([1, 2]\). Let's choose \( x_0 = 1.5 \).

The derivative of \( f(x) = x^5 - x - 1 \) is:
\[ f'(x) = 5x^4 - 1 \]

Step 2: First Iteration

Calculate the next approximation \( x_1 \):

\[ x_1 = x_0 - \frac{f(x_0)}{f'(x_0)} \]

For \( x_0 = 1.5 \):
\[ f(1.5) = (1.5)^5 - 1.5 - 1 = 7.59375 - 1.5 - 1 = 5.09375 \]
\[ f'(1.5) = 5(1.5)^4 - 1 = 5 \cdot 5.0625 - 1 = 25.3125 - 1 = 24.3125 \]

\[ x_1 = 1.5 - \frac{5.09375}{24.3125} \approx 1.2904 \]

Step 3: Second Iteration

Calculate the next approximation \( x_2 \):

\[ x_2 = x_1 - \frac{f(x_1)}{f'(x_1)} \]

For \( x_1 = 1.2904 \):
\[ f(1.2904) = (1.2904)^5 - 1.2904 - 1 \approx 3.1989 - 1.2904 - 1 = 0.9085 \]
\[ f'(1.2904) = 5(1.2904)^4 - 1 \approx 5 \cdot 2.7806 - 1 = 13.903 \]

\[ x_2 = 1.2904 - \frac{0.9085}{13.903} \approx 1.2250 \]

Final Answer

The approximate root of \( f(x) = x^5 - x - 1 \) in the interval \([1, 2]\) after three steps is \( x \approx 1.2250 \).

Key Concept

Newton's method is an iterative numerical method used to approximate the roots of a real-valued function.

Key Concept Explanation

Newton's method requires an initial guess and uses the derivative of the function to iteratively improve the guess. The method converges quickly if the initial guess is close to the actual root and the function behaves well (i.e., it is differentiable, and its derivative is not zero at the root).

Related Knowledge or Questions
[1] Explore the convergence criteria for Newton's method.
[2] Apply Newton's method to a different polynomial function.
[3] Investigate the impact of different initial guesses on the convergence of Newton's method.

---

### Part (b): \( f(x) = e^x - 2(x-1)^2 \) in the interval \([0, 1]\)

Step 1: Initial Guess and Derivative Calculation

Choose an initial guess \( x_0 \) within the interval \([0, 1]\). Let's choose \( x_0 = 0.5 \).

The derivative of \( f(x) = e^x - 2(x-1)^2 \) is:
\[ f'(x) = e^x - 4(x-1) \]

Step 2: First Iteration

Calculate the next approximation \( x_1 \):

\[ x_1 = x_0 - \frac{f(x_0)}{f'(x_0)} \]

For \( x_0 = 0.5 \):
\[ f(0.5) = e^{0.5} - 2(0.5-1)^2 = 1.6487 - 2(0.25) = 1.6487 - 0.5 = 1.1487 \]
\[ f'(0.5) = e^{0.5} - 4(0.5-1) = 1.6487 - 4(-0.5) = 1.6487 + 2 = 3.6487 \]

\[ x_1 = 0.5 - \frac{1.1487}{3.6487} \approx 0.1860 \]

Step 3: Second Iteration

Calculate the next approximation \( x_2 \):

\[ x_2 = x_1 - \frac{f(x_1)}{f'(x_1)} \]

For \( x_1 = 0.1860 \):
\[ f(0.1860) = e^{0.1860} - 2(0.1860-1)^2 \approx 1.2045 - 2 \cdot 0.6613 = 1.2045 - 1.3226 = -0.1181 \]
\[ f'(0.1860) = e^{0.1860} - 4(0.1860-1) \approx 1.2045 - 4(-0.8140) = 1.2045 + 3.256 = 4.4605 \]

\[ x_2 = 0.1860 - \frac{-0.1181}{4.4605} \approx 0.2125 \]

Final Answer

The approximate root of \( f(x) = e^x - 2(x-1)^2 \) in the interval \([0, 1]\) after three steps is \( x \approx 0.2125 \).

Key Concept

Newton's method is an iterative numerical method used to approximate the roots of a real-valued function.

Key Concept Explanation

Newton's method requires an initial guess and uses the derivative of the function to iteratively improve the guess. The method converges quickly if the initial guess is close to the actual root and the function behaves well (i.e., it is differentiable, and its derivative is not zero at the root).

Related Knowledge or Questions
[1] Explore the convergence criteria for Newton's method.
[2] Apply Newton's method to a different exponential function.
[3] Investigate the impact of different initial guesses on the convergence of Newton's method.

---

Well done on taking these steps to understand and solve the problem using Newton's method! Please let me know which related knowledge point or question you'd like to explore further, or feel free to ask any other questions you might have.

\section{Exam}

1. (6p.) Determine the limits, if the limit does not exist justify your answer
\begin{enumerate}
    \item[a.] \[\lim_{n \to \infty} \frac{\left(3n + 5\right)^{n^4}}{\left(3n - 2\right)^{n^4}}
\]

    \item[b.] 
\[
\lim_{x \to -\infty} \frac{\cos x}{x^2}
\]
\end{enumerate}

2. (6p.) Determine horizontal and vertical asymptotes of the function
\[ f(x) = \frac{2 - x^2}{e^x} \]

3. (6p.) Determine the intervals on which the function \( f \) increases or decreases, and the values \( x \in \mathbb{R} \), for which \( f \) attains its local extrema
\[ f(x) = xe^{-\frac{1}{2}x^2} \]

4. (6p.) Calculate the following integral
\[ \int \left( 2 + \frac{1}{1 + x^2} \arctan x \right) dx \]

5. (6p.) Sketch the finite region bounded by the following curves and calculate its area
\[ y = x(x - 3) \]\[ y = x - x^2 \]

\end{document}


\subsection{Continuity. Find values a, b.}


\subsection{Asymptotes. Find values a, b.}


\subsection{Monotonicity. Intervals}


\subsection{Integrals}


\subsection{Domain. Determine and sketch.}

\subsubsection{Problem 1}

\subsubsection*{    Step 1: Determine the Domain}

    The domain of a function \( f(x, y) \) is the set of all pairs \((x, y)\) for which the function is defined. For \( f(x, y) = \log_2(x^2y - 1) \) to be defined, the argument of the logarithm must be greater than zero because the logarithm of a non-positive number is undefined.

\[
x^2y - 1 > 0
\]
\[
x^2y > 1
\]
\[
y > \frac{1}{x^2}
\]

Thus, the domain of \( f \) is:

\[
D = \{ (x, y) \in \mathbb{R}^2 \mid y > \frac{1}{x^2} \}
\]

\subsubsection*{Step 2: Sketch the Domain}

The inequality \( y > \frac{1}{x^2} \) describes the region above the curve \( y = \frac{1}{x^2} \). This curve is a hyperbola that opens upwards. Below is the sketch of the domain:

\begin{figure}
    \centering
    \includegraphics[width=0.5\linewidth]{DomainGraph.png}
    \caption{Enter Caption}
    \label{fig:enter-label}
\end{figure}

\subsubsection*{Step 3: Find the First Order Partial Derivatives}

To find the first order partial derivatives, we will use the chain rule and properties of logarithms.

\subsubsection*{Partial derivative with respect to \( x \):}

\[
f(x, y) = \log_2(x^2y - 1)
\]

First, apply the chain rule:
\[
\frac{\partial f}{\partial x} = \frac{d}{dx} \left[ \log_2(u) \right] \cdot \frac{\partial u}{\partial x}
\]

where \( u = x^2y - 1 \). The derivative of \( \log_2(u) \) is:
\[
\frac{d}{du} \left[ \log_2(u) \right] = \frac{1}{u \ln(2)}
\]

The derivative of \( u \) with respect to \( x \) is:
\[
\frac{\partial u}{\partial x} = \frac{\partial}{\partial x} (x^2y - 1) = 2xy
\]

So,
\[
\frac{\partial f}{\partial x} = \frac{1}{(x^2y - 1) \ln(2)} \cdot 2xy = \frac{2xy}{(x^2y - 1) \ln(2)}
\]

\subsubsection*{Partial derivative with respect to \( y \):}

Similarly, for \( y \),
\[
\frac{\partial f}{\partial y} = \frac{d}{dy} \left[ \log_2(u) \right] \cdot \frac{\partial u}{\partial y}
\]

The derivative of \( u \) with respect to \( y \) is:
\[
\frac{\partial u}{\partial y} = \frac{\partial}{\partial y} (x^2y - 1) = x^2
\]

So,
\[
\frac{\partial f}{\partial y} = \frac{1}{(x^2y - 1) \ln(2)} \cdot x^2 = \frac{x^2}{(x^2y - 1) \ln(2)}
\]

\subsubsection*{Final Answer}

1. \textbf{Domain of \( f \)}: \( \{ (x, y) \in \mathbb{R}^2 \mid y > \frac{1}{x^2} \} \)

2. \textbf{First Order Partial Derivatives}:
   \[
   \frac{\partial f}{\partial x} = \frac{2xy}{(x^2y - 1) \ln(2)}
   \]
   \[
   \frac{\partial f}{\partial y} = \frac{x^2}{(x^2y - 1) \ln(2)}
   \]

\subsubsection*{Key Concept}

The key concept involved in this problem is understanding the domain of a logarithmic function and computing the first order partial derivatives using the chain rule.

\subsubsection*{Key Concept Explanation}

1. \textbf{Domain of Logarithmic Functions}:
   For the logarithm \( \log_b(x) \) to be defined, \( x \) must be greater than zero. This is because the logarithm of zero or a negative number is undefined in the real number system.
   
2. \textbf{Partial Derivatives and Chain Rule}:
   Partial derivatives measure how a function changes as each variable changes, holding the other variables constant. The chain rule is used to differentiate composite functions. If \( z = f(u) \) and \( u = g(x, y) \), then the partial derivatives are found by multiplying the derivative of the outer function by the derivative of the inner function with respect to the variable of interest.

\subsubsection*{Related Knowledge or Questions}

\begin{enumerate}
    \item Determine the second order partial derivatives of \( f(x, y) = \log_2(x^2y - 1) \).
    \item Find the critical points of \( f(x, y) = \log_2(x^2y - 1) \) and classify them.
    \item Evaluate the double integral \( \iint_D f(x, y) \, dA \) where \( D \) is the domain of \( f \).
\end{enumerate}



\end{document}






