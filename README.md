
# The few-books dataset

This is a list of links to scanned pdf math books, a small but useful corpus.

Reading mathematics books is an indispensable part of learning university-level mathematics. These textbooks take a lot of time to read, but they contain detailed proofs that are not in summary articles like wikipedia or blogs. The books are curcial for the knowledge-heavy field of math.

However, many classic mathematics books are likely absent from the current training data of LLMs (large language models). Datasets like CommonCrawl and FineWeb are derived from HTML-based websites, and therefore miss most books. The Books3 subset of RedPajama includes a lot of fiction and non-fiction works. However, most of these books likely originate from EPUB e-book files, whereas classic mathematics texts are often only distributed in PDF format—often as scanned copies.

Incorporating these books systematically into the training data could significantly enhance an LLM's understanding of advanced mathematics, improve expert user experience, and might dramatically change evaluation results in chain-of-thought and theorem prover integration, simply by eliminating the lack of knowledge.

Unlike broad "calorie-rich" datasets, these high-quality books are more like "vitamins". They are a really small part of available data, but human experts engage with them daily.

Below are several links to mathematics books in PDF format that I gathered via Google search. You can download these small pdf files with a Python script. I tried to (more or less) order the book links by prerequisite, so we can train the model with the more basic knowledge first, ie try doing curriculum learning.

Many of these books do not have an available Latex version on the Internet, so some form of OCR is needed. With the advance of vision-language models, we can now prompt them to recognize formulas and organize a markdown version. This might give a more consistant and cheaper OCR result, compared to previous technologies like MathPix.

I referred to these book lists:  
- https://www.ocf.berkeley.edu/~abhishek/chicmath.htm  
- https://github.com/rossant/awesome-math  
- https://github.com/zhangir-azerbayev/proof-pile/blob/main/fetch_books_and_formal.py  

Other training data to consider:  
- Contest problems from AoPS (Art of Problem Solving) like the MATH dataset or [this one](https://huggingface.co/datasets/di-zhang-fdu/AOPS/viewer/default/train?row=0&views%5B%5D=train)  
- GTM (Graduate Texts in Mathematics) book series with about 300 books (Also UTM, GSM)  
- Wiki websites: Wikipedia, ProofWiki, PlanetMath, nLab
- QA datasets: MathOverflow, MathStackExchange  
- Github repos: Theorem provers (source code, textbooks, standard libraries, projects)
- Plug-and-Chug or auto-generated problems: MathQA, DeepMind Mathematics

---

# High School and Problem Solving

Euclid, Elements https://www.gutenberg.org/files/21076/21076-t/21076-t.tex

Lehoczky and Rusczyk, The Art of Problem Solving - Volume 1: the Basics https://github.com/lasikaspur/The-art-of-problem-solving.-Volume-1-The-basics-PDFDrive-/blob/main/The%20art%20of%20problem%20solving.%20Volume%201%2C%20The%20basics%20(%20PDFDrive%20).pdf

Arthur Engel, Problem-Solving Strategies https://mathematicalolympiads.wordpress.com/wp-content/uploads/2012/08/75427434-problem-books-in-mathematics-problem-solving-strategies.pdf

Terrece Tao, Solving Mathematical Problems https://raktimchatterjee.wordpress.com/wp-content/uploads/2015/09/solving-mathematical-problems-terence-tao.pdf


# Center of College Math 

## Introduction to Math
Evan Chen, An Infinitely Large Napkin https://venhance.github.io/napkin/Napkin.pdf

Gowers, Princeton Companion to Mathematics https://sites.math.rutgers.edu/~zeilberg/akherim/PCM.pdf
Hilbert, Foundations of geometry https://math.berkeley.edu/~wodzicki/160/Hilbert.pdf

Graham, Concrete mathematics https://github.com/djtrack16/thyme/blob/master/math/Concrete%20Mathematics%20A%20Foundation%20of%20Computer%20Science%202nd%20Edition.pdf

Halmos, Naive set theory http://people.whitman.edu/~guichard/260/halmos__naive_set_theory.pdf

## Precalculus
...

## Calculus
...

## Linear Algebra

Gilbert Strang, Linear Algebra and Its Applications
https://rksmvv.ac.in/wp-content/uploads/2021/04/Gilbert_Strang_Linear_Algebra_and_Its_Applicatio_230928_225121.pdf

Sheldon Axler, Linear Algebra Done Right https://linear.axler.net/LADR4e.pdf

## Probability and Statistics
...


## Mathematical Analysis

Terence Tao, Analysis https://math.unm.edu/~crisp/courses/math401/tao.pdf Solutions https://github.com/frederic-santos/taoanalysissolutions/blob/master/analysis_t1_exercises.tex https://github.com/frederic-santos/taoanalysissolutions/blob/master/analysis_t2_exercises.tex

Stephen Abbott, Understanding Analysis https://books.tarbaweya.org/static/documents/uploads/pdf/2015_Book_UnderstandingAnalysis.pdf

Charles C. Pugh, Real Mathematical Analysis https://smartmanmaths.wordpress.com/wp-content/uploads/2017/11/real-mathematical-analysis.pdf

Richard R. Goldberg, Methods of Real Analysis https://alansinyal.wordpress.com/wp-content/uploads/2012/08/method-of-real-analysis.pdf

Tom M. Apostol, Mathematical Analysis https://invent.ilmkidunya.com/images/Section/mathematical-analysis-css-book.pdf

Rudin, Principles of Mathematical Analysis https://david92jackson.neocities.org/images/Principles_of_Mathematical_Analysis-Rudin.pdf Solutions https://pages.cs.wisc.edu/~wentaowu/other-docs/POMA_Solution_Sheet.pdf https://github.com/awasthi/math-solutions/blob/master/Rudin/Principles%20of%20Mathematical%20Analysis/RudinSolutions.tex

Gelbaum, Counterexamples in Analysis https://faculty.ksu.edu.sa/sites/default/files/_olmsted_1.pdf

## Real Analysis

Elias Stein & Rami Shakarchi, Real Analysis: Measure Theory, Integration, and Hilbert Spaces https://www.cmat.edu.uy/~mordecki/courses/medida2013/book.pdf

Gerald B. Folland, Real Analysis: Modern Techniques and Their Applications https://apachepersonal.miun.se/~andrli/Bok.pdf

Serge Lang, Real and Functional Analysis https://59clc.wordpress.com/wp-content/uploads/2012/08/real-and-functional-analysis-lang.pdf

H. L. Royden & P. M. Fitzpatrick - Real Analysis https://s2pnd-matematika.fkip.unpatti.ac.id/wp-content/uploads/2019/03/Real-Analysis-4th-Ed-Royden.pdf

Rudin, Real and Complex Analysis https://59clc.wordpress.com/wp-content/uploads/2011/01/real-and-complex-analysis.pdf Solutions https://iseulbee.com/wp-content/uploads/2014/03/RCA-Solution.pdf https://github.com/awasthi/math-solutions/blob/master/Rudin/Real%20and%20Complex%20Analysis/PapaRudinSolutions.tex

## Complex Variables
Conway, Functions of One Complex Variable https://psm73.wordpress.com/wp-content/uploads/2009/03/conway.pdf

## Ordinary Differential Equations
Arnold, Ordinary differential equations https://loshijosdelagrange.wordpress.com/wp-content/uploads/2013/04/vladimir-i-arnold-vladimir-i-arnold-roger-cooke-ordinary-differential-equations-1992.pdf  

## Point Set Topology
Munkres, Topology https://people.math.ethz.ch/~dkosanovic/24-FS/Munkres-Topology.pdf Solutions https://math-study.net/wp-content/TopologySolutions.pdf https://math.ucr.edu/~res/math205B-2021/solutions/gentop-solutions.pdf https://github.com/awasthi/math-solutions/blob/master/Munkres/Munkres%20Solutions.tex

Armstrong, Basic Topology https://math.mit.edu/~hrm/palestine/armstrong-basic-topology.pdf Solutions https://github.com/gblikas/armstrongTopologySolutions/blob/master/Armstrong_Topology_Solutions%20(1).pdf

Kelley, General Topology https://cjhb.site/Files.php/Books/(Uncategorized)/General%20Topology-John%20L.Kelley.pdf

Morris, Topology without Tears, https://www.topologywithouttears.net/topbook.pdf

Lynn Arthur Steen & J. Arthur Seebach, Counterexamples in Topology, https://editorialdinosaurio.wordpress.com/wp-content/uploads/2012/03/counterexamples_in_topology_-_l-_steen__j-_seebach__1970__ww.pdf

Viro, Elementary Topology Problem Textbook https://www.maths.ed.ac.uk/~v1ranick/papers/viro.pdf

Matsumura, Introduction to Topology [lecture-notes] https://pi.math.cornell.edu/~matsumura/math4530/IntroToTopology.pdf

Renzo, Introduction to Topology [lecture-notes] https://www.math.colostate.edu/~renzo/teaching/Topology10/Notes.pdf

Warner, Topological Rings, https://mezbanhabibi.ir/wp-content/uploads/2020/01/Topological-Rings-Warner.pdf

## Algebra
Artin, Algebra https://media.githubusercontent.com/media/storagelfs/books/main/Applied%20Mathematics/Algebra/Artin.%20Algebra.%201991.pdf Solutions https://github.com/awasthi/math-solutions/blob/master/Artin/Artin%20Solutions.tex

Paolo Aluffi, Algebra: Chapter 0 https://agorism.dev/book/math/alg/algebra_chapter-0_paolo-aluffi.pdf








# Applied Fields, Computational Fields, Combinatorics

## Mathematical Modeling
...

## Numerical Computing

Timothy Sauer, Numerical Analysis https://eclass.aueb.gr/modules/document/file.php/MISC249/Sauer%20-%20Numerical%20Analysis%202e.pdf

Horm, Matrix Analysis https://www.anandinstitute.org/pdf/Roger_A.Horn.%20_Matrix_Analysis_2nd_edition(BookSee.org).pdf

Nocedal, Numerical Optimization
https://www.math.uci.edu/~qnie/Publications/NumericalOptimization.pdf

Boyd, Convex Optimization https://web.stanford.edu/~boyd/cvxbook/bv_cvxbook.pdf

## Fourier Analysis and Signal Processing


## Finite Element Method
...

## Combinatorics

Sagan, Combinatorics: The Art of Counting https://users.math.msu.edu/users/bsagan/Books/Aoc/final.pdf

## Enumerative Combinatorics
Stanley, Enumerative Combinatorics https://www.ms.uky.edu/~sohum/putnam/enu_comb_stanley.pdf

Grinberg, Enumerative Combinatorics: class notes https://www.cip.ifi.lmu.de/~grinberg/t/19fco/n/n.pdf

Cameron, Notes on Counting: An Introduction to Enumerative Combinatorics https://webspace.maths.qmul.ac.uk/b.jackson/MTHM030/counting.pdf

Yan, Handbook of Enumerative Combinatorics https://people.tamu.edu/~huafei-yan//Files/Yan-Final-Own-Copy.pdf

Ardila, Algebraic and geometric methods in enumerative combinatorics https://fardila.com/Articles/methods.pdf


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










# More Analysis

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


# More Algebra and Geometry

## Differential Geometry
Spivak, Calculus on Manifolds http://strangebeautiful.com/other-texts/spivak-calc-manifolds.pdf

Spivak, A comprehensive introduction to differential geometry, 1 https://ia601401.us.archive.org/9/items/X8Q8QXH8UH189HX98XQ/%5BMichael_Spivak%5D_A_Comprehensive_Introduction_to_D1%28BookZZ.org%29.pdf

## Riemann Geometry
Jost, Compact Riemann surfaces https://www.maths.ed.ac.uk/~v1ranick/papers/jost.pdf

## Algebraic Topology
Hatcher, Algebraic Topology https://pi.math.cornell.edu/~hatcher/AT/AT.pdf Solutions https://github.com/awasthi/math-solutions/blob/master/Hatcher/Hatcher%20Solutions.tex

## Differential Topology
J. W. Milnor and J. D. Stasheff, Characteristic Classes https://aareyanmanzoor.github.io/assets/books/characteristic-classes.pdf Solutions https://github.com/awasthi/math-solutions/blob/master/Milnor/Milnor.tex

## Low-Dimensional Topology
...

## Combintorial Topology
...

## Topological Data Analysis

An introduction to Topological Data Analysis: fundamental and practical aspects for data scientists https://arxiv.org/pdf/1710.04019

Computational Topology for Data Analysis https://www.cs.purdue.edu/homes/tamaldey/book/CTDAbook/CTDAbook.pdf

Topological Data Analysis Mastermath [lecture-notes] https://www.few.vu.nl/~botnan/lecture_notes.pdf

Zomorodian, Topological Data Analysis https://www.datascienceassn.org/sites/default/files/Topological%20Data%20Analysis.pdf

Topological Data Analysis https://www.math.columbia.edu/~thaddeus/blumberg/book/07.2_pp_122_169_Topological_Data_Analysis.pdf

Moschen, Topological Data Analysis - Exercises https://lucasmoschen.github.io/files/disciplines/topological-data-analysis/exercises.pdf

Schenck, Algebraic Foundations for Applied Topology and Data Analysis https://webhome.auburn.edu/~hks0015/data2.pdf

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

Jiri Adámek, Horst Herrlich, George E. Strecker — Abstract and Concrete Categories: The Joy of Cats http://www.tac.mta.ca/tac/reprints/articles/17/tr17.pdf

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

