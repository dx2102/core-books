
# The few-books dataset

Reading mathematics books is an indispensable part of learning university-level mathematics. These textbooks take a lot of time to read, but they contain detailed proofs that are not in summary articles like wikipedia or blogs. The books are curcial for the knowledge-heavy field of math.

However, many classic mathematics books are likely absent from the current training data of LLMs (large language models). Datasets like CommonCrawl and FineWeb are derived from HTML-based websites, and therefore miss most books. The Books3 subset of RedPajama includes a lot of fiction and non-fiction works. However, most of these books likely originate from EPUB e-book files, whereas classic mathematics texts are often only distributed in PDF format—often as scanned copies.

Incorporating these books systematically into the training data could significantly enhance an LLM's understanding of advanced mathematics, improve expert user experience, and might dramatically change evaluation results in chain-of-thought and theorem prover integration, simply by eliminating the lack of knowledge.

Unlike broad "calorie-rich" datasets, these high-quality books are more like "vitamins". They are a really small part of available data, but human experts engage with them daily.

Below are several links to mathematics books in PDF format that I gathered via Google search. You can download these small pdf files with a Python script. I tried to (more or less) order the book links by prerequisite, so we can train the model with the more basic knowledge first, ie try doing curriculum learning.

Many of these books do not have an available Latex version on the Internet, so some form of OCR is needed. With the advance of vision-language models, we can now prompt them to recognize formulas and organize a markdown version. This might give a more consistant and cheaper OCR result, compared to previous technologies like MathPix.

I referred to these book lists:  
https://www.ocf.berkeley.edu/~abhishek/chicmath.htm  
https://github.com/rossant/awesome-math  
https://github.com/zhangir-azerbayev/proof-pile/blob/main/fetch_books_and_formal.py  

Other training data to consider:  
Contest problems from AoPS (Art of Problem Solving) like: https://huggingface.co/datasets/di-zhang-fdu/AOPS/viewer/default/train?row=0&views%5B%5D=train  
GTM (Graduate Texts in Mathematics) book series with about 200 books  
Wiki websites like: Wikipedia, ProofWiki, PlanetMath, nLab  
Github repos: Theorem provers (source code, textbooks, standard libraries, projects)  

---

# High School and Problem Solving

Euclid, Elements https://www.gutenberg.org/files/21076/21076-pdf.pdf

Lehoczky and Rusczyk, The Art of Problem Solving, Volume 1: the Basics https://github.com/lasikaspur/The-art-of-problem-solving.-Volume-1-The-basics-PDFDrive-/blob/main/The%20art%20of%20problem%20solving.%20Volume%201%2C%20The%20basics%20(%20PDFDrive%20).pdf

Arthur Engel, Problem-Solving Strategies https://mathematicalolympiads.wordpress.com/wp-content/uploads/2012/08/75427434-problem-books-in-mathematics-problem-solving-strategies.pdf

Terrece Tao, Solving Mathematical Problems https://raktimchatterjee.wordpress.com/wp-content/uploads/2015/09/solving-mathematical-problems-terence-tao.pdf


# Beginning of College Math

## Transition to College Math
Evan Chen, An Infinitely Large Napkin https://venhance.github.io/napkin/Napkin.pdf

Hilbert, Foundations of geometry https://math.berkeley.edu/~wodzicki/160/Hilbert.pdf

Knuth, Concrete mathematics https://github.com/djtrack16/thyme/blob/master/math/Concrete%20Mathematics%20A%20Foundation%20of%20Computer%20Science%202nd%20Edition.pdf

Halmos, Naive set theory http://people.whitman.edu/~guichard/260/halmos__naive_set_theory.pdf

## Calculus
...

## Linear Algebra

Gilbert Strang, Linear Algebra and Its Applications
https://rksmvv.ac.in/wp-content/uploads/2021/04/Gilbert_Strang_Linear_Algebra_and_Its_Applicatio_230928_225121.pdf

Sheldon Axler, Linear Algebra Done Right https://linear.axler.net/LADR4e.pdf

## Probability and Statistics
...



# Relatively Independent Fields

## Mathematical Modeling
...

## Numerical Computing

Timothy Sauer, Numerical Analysis https://eclass.aueb.gr/modules/document/file.php/MISC249/Sauer%20-%20Numerical%20Analysis%202e.pdf

Horm, Matrix Analysis https://www.anandinstitute.org/pdf/Roger_A.Horn.%20_Matrix_Analysis_2nd_edition(BookSee.org).pdf

Nocedal, Numerical Optimization
https://www.math.uci.edu/~qnie/Publications/NumericalOptimization.pdf

Boyd, Convex Optimization https://web.stanford.edu/~boyd/cvxbook/bv_cvxbook.pdf

## Finite Element Method
...

## Combinatorics
...

## Enumerative Combinatorics
...

## Graph Theory
...

## Spectral Graph Theory
...

## Ramsey Theory
...

## Information Theory
...

## Control Theory
...

## Coding Theory
...

## Game Theory
...

## Algorithms
...

## Algorithmic Complexity
...

## Theory of Computation
...

## Quantum Computing
...

## SAT Solving and Theorem Proving
...

## Elementary Number Theory
...

## Cryptography
...

## Computational Geometry
...

## Discrete and Combinatorial Geometry
...









# Core of Math
## Mathematical Analysis

Terence Tao, Analysis https://math.unm.edu/~crisp/courses/math401/tao.pdf

Gelbaum, Counterexamples in Analysis https://faculty.ksu.edu.sa/sites/default/files/_olmsted_1.pdf

Rudin, Real and Complex Analysis https://59clc.wordpress.com/wp-content/uploads/2011/01/real-and-complex-analysis.pdf

## Complex Variables
Conway, Functions of One Complex Variable https://psm73.wordpress.com/wp-content/uploads/2009/03/conway.pdf

## Ordinary Differential Equations
Arnold, Ordinary differential equations https://loshijosdelagrange.wordpress.com/wp-content/uploads/2013/04/vladimir-i-arnold-vladimir-i-arnold-roger-cooke-ordinary-differential-equations-1992.pdf

## Point Set Topology
Munkres, Topology https://people.math.ethz.ch/~dkosanovic/24-FS/Munkres-Topology.pdf

Armstrong, Basic Topology https://math.mit.edu/~hrm/palestine/armstrong-basic-topology.pdf

## Algebra
Artin, Algebra https://media.githubusercontent.com/media/storagelfs/books/main/Applied%20Mathematics/Algebra/Artin.%20Algebra.%201991.pdf

Paolo Aluffi, Algebra: Chapter 0 https://agorism.dev/book/math/alg/algebra_chapter-0_paolo-aluffi.pdf

# Advanced Analysis

## Mathematical Methods in Physics
...

## Special Functions
...

## Functional Analysis
Erwin Kreyszig, Introductory functional analysis with applications https://asoimatepn.wordpress.com/wp-content/uploads/2015/04/kreyszig-erwin-introductory-functional-analysis-with-aplications-university-of-windsor-wiley-classics-library-usa-1989.pdf

Walter Rudin, Functional analysis https://59clc.wordpress.com/wp-content/uploads/2012/08/functional-analysis-_-rudin-2th.pdf

Peter Lax, Functional analysis http://users.math.uoc.gr/~frantzikinakis/FunctionalGrad2015/Lax.pdf

Kadison/Ringrose, Fundamentals of the theory of operator algebras
http://lib.ysu.am/disciplines_bk/d06f33909cd098cbca3d9a22596fd772.pdf

## Partial Differential Equations

Taylor, Partial differential equations I: basic theory https://link.springer.com/content/pdf/10.1007/978-3-031-33859-5.pdf

Evans, Partial differential equations https://math24.wordpress.com/wp-content/uploads/2013/02/partial-differential-equations-by-evans.pdf

## Mathematical Physics
...

## Harmonic Analysis
...

## Operator Theory
...

## Measure Theory
...

## Geometric Measure Theory
...

## Probability Theory
...

## Mathematical Statistics
...

## Stochastic Processes
...

## Dynamical Systems
...

## Ergodic Theory
...

## Fractal Geometry
...

## Symplectic Dynamics
...


# Advanced Algebra and Geometry

## Differential Geometry
Spivak, Calculus on Manifolds http://strangebeautiful.com/other-texts/spivak-calc-manifolds.pdf

Spivak, A comprehensive introduction to differential geometry, 1 https://ia601401.us.archive.org/9/items/X8Q8QXH8UH189HX98XQ/%5BMichael_Spivak%5D_A_Comprehensive_Introduction_to_D1%28BookZZ.org%29.pdf

## Riemann Geometry
Jost, Compact Riemann surfaces https://www.maths.ed.ac.uk/~v1ranick/papers/jost.pdf

## Algebraic Topology
...

## Low-Dimensional Topology
...

## Combintorial Topology
...

## Topological Data Analysis
...

## Quantum Topology
...

## Complex Geometry
...

## Representation Theory
Fulton/Harris, Representation theory: a first course https://mat.uab.cat/~pitsch/ReadingSeminar/Fulton-Harris.pdf

## Lie Groups
...

## Finite Group Theory
...

## Algebraic Combinatorics
...

## Homological Algebra
...

## Commutative Algebra
...

## Category Theory
...

## Symplectic Geometry
...

## Analytic Number Theory
...

## Algebraic Number Theory
...

## Algebraic Geometry
Robin Hartshorne, Algebraic Geometry https://www.math.stonybrook.edu/~kamenova/homepage_files/Hartshorne_engl.pdf

Stacks Project https://stacks.math.columbia.edu/download/book.pdf

## K-Theory
...

## Elliptic Curves
...

## Modular Forms
...

## p-adic Analysis
...

## Iwasawa Theory
...

## Arithmetic Geometry
...

## Noncommutative Geometry
...

### Additional books collected by others:
!repo-with-pdf: https://github.com/Rafiquzzaman420/Math-Books

!repo-with-readme-links: https://github.com/rossant/awesome-math

# Other Advanced Books 

### GTM (Graduate Texts in Mathematics) Series

!repo-with-pdf：https://github.com/chanqi4444/GTM


### By Terence Tao

Terence Tao, Introduction to Measure Theory https://terrytao.wordpress.com/wp-content/uploads/2012/12/gsm-126-tao5-measure-book.pdf

Terence Tao, Topics in random matrix theory https://terrytao.wordpress.com/wp-content/uploads/2011/02/matrix-book.pdf

Terence Tao, Additive Combinatorics
http://math.bme.hu/~gabor/oktatas/SztoM/TaoVu.AddComb.pdf

Terence Tao, Nonlinear dispersive equations: local and global analysis https://www.math.ucla.edu/~tao/preprints/chapter.pdf

Terence Tao, Hilbert’s fifth problem and related topics https://terrytao.wordpress.com/wp-content/uploads/2012/03/hilbert-book.pdf

