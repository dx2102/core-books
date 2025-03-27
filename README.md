
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

Daniel J. Velleman, How to Prove It https://users.metu.edu.tr/serge/courses/111-2011/textbook-math111.pdf

Graham, Concrete mathematics https://github.com/djtrack16/thyme/blob/master/math/Concrete%20Mathematics%20A%20Foundation%20of%20Computer%20Science%202nd%20Edition.pdf

Halmos, Naive set theory http://people.whitman.edu/~guichard/260/halmos__naive_set_theory.pdf

## Calculus

Tom M. Apostol, Calculus Vol. 1   https://theswissbay.ch/pdf/Gentoomen%20Library/Maths/Calculus/Tom%20Apostol%20-%20Calculus%20vol.1%20-%20One-variable%20Calculus%2C%20with%20an%20Introduction%20to%20Linear%20Algebra%20%281975%29.pdf

Tom M. Apostol, Calculus Vol. 2   https://theswissbay.ch/pdf/Gentoomen%20Library/Maths/Calculus/Tom%20Apostol%20-%20Calculus%20Vol.2%20-%20Multi-Variable%20Calculus%20and%20Linear%20Algebra%20with%20Applications.pdf

Michael Spivak, Calculus   http://148.216.54.18/~fhernandez/Cursos/Calculo2015/spivak.pdf

James Stewart, Calculus   https://patemath.weebly.com/uploads/5/2/5/8/52589185/james-stewart-calculus-early-transcendentals-7th-edition-2012-1-20ng7to-1ck11on.pdf

Jerrold E. Marsden & Alan Weinstein, Calculus Vol. 1   https://valle.fciencias.unam.mx/librosautor/CU.pdf

Jerrold E. Marsden & Alan Weinstein, Calculus Vol. 2   https://valle.fciencias.unam.mx/librosautor/CU.pdf

Howard Anton, Calculus   https://3lihandam69.files.wordpress.com/2018/10/calculus-10th-edition-anton.pdf

Ron Larson & Bruce Edwards, Calculus   https://github.com/bookyue/my_books/blob/master/mathematics/calculus/larson_calculus/Calculus%2011th%20edition%20by%20Ron%20Larson%2C%20Bruce%20Edwards.pdf

Richard Courant & Fritz John, Introduction to Calculus and Analysis Vol. 1   http://www.astrosen.unam.mx/~aceves/Metodos/ebooks/courant_john1.pdf

Richard Courant & Fritz John, Introduction to Calculus and Analysis Vol. 2   http://www.astrosen.unam.mx/~aceves/Metodos/ebooks/courant_john1.pdf

Edwin E. Moise & Floyd L. Downs Jr., Calculus   https://colmaths.files.wordpress.com/2013/01/geometria-moderna-moise.pdf

James Kaplansky, An Introduction to Differential and Integral Calculus https://www.maths.cam.ac.uk/undergrad/files/schedules.pdf

## Linear Algebra

David C. Lay, Linear Algebra and Its Applications   https://broman.dev/download/Linear%20Algebra%20and%20its%20Applications%205th%20Edition.pdf

Gilbert Strang, Introduction to Linear Algebra   https://students.aiu.edu/submissions/profiles/resources/onlineBook/Y5B7M4_Introduction_to_Linear_Algebra-_Fourth_Edition.pdf

Gilbert Strang, Linear Algebra and Its Applications   https://rksmvv.ac.in/wp-content/uploads/2021/04/Gilbert_Strang_Linear_Algebra_and_Its_Applicatio_230928_225121.pdf

Sheldon Axler, Linear Algebra Done Right   https://linear.axler.net/LADR4e.pdf

Sergei Treil, Linear Algebra Done Wrong   https://www.math.brown.edu/streil/papers/LADW/LADW-2014-09.pdf

Stephen H. Friedberg, Linear Algebra   https://anandinstitute.org/pdf/lenearal.pdf

Serge Lang, Linear Algebra   https://users.math.msu.edu/users/parker/309/Lang-linear-algebra.pdf

Kenneth Hoffman & Ray Kunze, Linear Algebra   https://www.math.pku.edu.cn/teachers/anjp/textbook.pdf

Paul R. Halmos, Finite-Dimensional Vector Spaces   https://www.magradze.de/academics/CS550/Halmos.pdf

Steven Roman, Advanced Linear Algebra   https://s2pnd-matematika.fkip.unpatti.ac.id/wp-content/uploads/2019/03/Graduate-Texts-in-Mathematics-135-Steven-Roman-Advanced-Linear-Algebra-Third-Edition-Graduate-Texts-in-Mathematics-Springer-2008.pdf

Seymour Lipschutz & Marc Lipson, Schaum’s Outline of Linear Algebra http://www.astronomia.edu.uy/progs/algebra/Linear_Algebra,_4th_Edition__(2009)Lipschutz-Lipson.pdf

## Probability Theory

William Feller, An Introduction to Probability Theory and Its Applications Vol. 1   https://bitcoinwords.github.io/assets/papers/an-introduction-to-probability-theory-and-its-applications.pdf

William Feller, An Introduction to Probability Theory and Its Applications Vol. 2   https://www.climet.com/toolbox/feller-correction-calculator/Feller-1968.pdf

A. A. Borovkov, Probability Theory http://repository.cinec.edu/bitstream/cinec20/1178/1/2013_Book_ProbabilityTheory.pdf

Patrick Billingsley, Probability and Measure https://www.colorado.edu/amath/sites/default/files/attached-files/billingsley.pdf

Loève, Probability Theory https://math.mit.edu/~hrm/palestine/maclane-categories.pdf

Jeffrey S. Rosenthal, A First Look at Rigorous Probability Theory https://tiu-edu.uz/media/books/2024/05/28/1664973378.pdf

Jean Jacod & Philip Protter, Probability Essentials   https://www.karlin.mff.cuni.cz/~lachout/Vyuka/O-Sem/JacodProtter2004.pdf

Yuan Shih Chow & Henry Teicher, Probability Theory: Independence, Interchangeability, Martingales   http://ndl.ethernet.edu.et/bitstream/123456789/37744/1/Yuan%20Shih%20Chow_1997.pdf

S. M. Ross, Stochastic Processes https://github.com/anishLearnsToCode/books/blob/master/probability-statistics/Stochastic-Processes-sheldon-m-ross.pdf

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

Lars Ahlfors, Complex Analysis https://mccuan.math.gatech.edu/courses/6321/lars-ahlfors-complex-analysis-third-edition-mcgraw-hill-science_engineering_math-1979.pdf

Conway, Functions of One Complex Variable https://psm73.wordpress.com/wp-content/uploads/2009/03/conway.pdf

Theodore W. Gamelin, Complex Analysis https://unina2.on-line.it/sebina/repository/catalogazione/documenti/Gamelin%20-%20Complex%20analysis.pdf

Reinhold Remmert, Theory of Complex Functions https://www.matem.unam.mx/~hector/Remmert-TheoryCpxFtns.pdf

Serge Lang, Complex Analysis http://79.175.134.118/portals/0/books/gtm/شمارهٔ%20۱%DB%B0۳-آنالیز%20مختلط،%20سرژ%20لنگ%20(1999،%20ویرایش%20چهارم).pdf

Elias Stein & Rami Shakarchi, Complex Analysis https://www.fing.edu.uy/~cerminar/Complex_Analysis.pdf

Mark J. Ablowitz & Athanassios S. Fokas, Complex Variables: Introduction and Applications https://ftfsite.ru/wp-content/files/tfkp_endlish_2.2.pdf

James Ward Brown & Ruel V. Churchill, Complex Variables and Applications https://people.math.sc.edu/girardi/m7034/book/ChurchillBrown8ed.pdf

Donald Sarason, Complex Function Theory https://www.ams.org/books/mbk/049/mbk049-endmatter.pdf

Eberhard Freitag, Complex Analysis https://www.mathi.uni-heidelberg.de/~freitag/skripten/complexspaces.pdf


## Ordinary Differential Equations

Earl Coddington, An Introduction to Ordinary Differential Equations   https://www.iitg.ac.in/jiten/Extra/Coddrington.pdf

E.L. Ince, Ordinary Differential Equations   https://msulaiman.org/onewebmedia/(UNITEXT%2088)%20Shair%20Ahmad,%20Antonio%20Ambrosetti%20(auth.)-A%20Textbook%20on%20Ordinary%20Differential%20Equations-Springer%20International%20Publishing%20(2015).pdf

William E. Boyce & Richard C. DiPrima, Elementary Differential Equations and Boundary Value Problems   https://scienceclopedia.wordpress.com/wp-content/uploads/2019/09/william-e.-boyceelementary-differential-equations-and-boundary-value-problems-wiley-2017.pdf

George F. Simmons, Differential Equations with Applications and Historical Notes   https://horizons-2000.org/92.%20Misc%20Files/Reading/Differential%20Equations--George%20Simpson.pdf

Dennis G. Zill, A First Course in Differential Equations   http://lya.fciencias.unam.mx/jele/EDOs2k15.2/Libros/A%20First%20Course%20in%20Differential%20Equations%20with%20Modeling%20Applications%2010e%202012%20Zill.pdf

Paul Blanchard, Robert L. Devaney & Glen R. Hall, Differential Equations   http://students.aiu.edu/submissions/profiles/resources/onlineBook/P6E5w8_differential%20equations%20blanchard%204th.pdf

Morris Tenenbaum & Harry Pollard, Ordinary Differential Equations   https://cosmathclub.files.wordpress.com/2014/10/morris-tenenbaum-harry-pollard-ordinary-differential-equations-copy.pdf

Martin Braun, Differential Equations and Their Applications   https://www.mmcmodinagar.ac.in/econtent/physics/DifferentialEquationsAndTheirApplications.pdf

V.I. Arnold, Ordinary Differential Equations   https://loshijosdelagrange.files.wordpress.com/2013/04/vladimir-i-arnold-vladimir-i-arnold-roger-cooke-ordinary-differential-equations-1992.pdf

Shepley L. Ross, Differential Equations   http://debracollege.dspaces.org/bitstream/123456789/19/1/Ross.pdf

Tyn Myint-U & Lokenath Debnath, Linear Partial Differential Equations for Scientists and Engineers https://sharif.ir/~moosavi/Myint-U_Debnath-Linear_Partial_Differential_Equations_for_Scientists_and_Engineers.pdf


## Point Set Topology

Munkres, Topology https://people.math.ethz.ch/~dkosanovic/24-FS/Munkres-Topology.pdf Solutions https://math-study.net/wp-content/TopologySolutions.pdf https://math.ucr.edu/~res/math205B-2021/solutions/gentop-solutions.pdf https://github.com/awasthi/math-solutions/blob/master/Munkres/Munkres%20Solutions.tex

Armstrong, Basic Topology https://math.mit.edu/~hrm/palestine/armstrong-basic-topology.pdf Solutions https://github.com/gblikas/armstrongTopologySolutions/blob/master/Armstrong_Topology_Solutions%20(1).pdf

Kelley, General Topology https://cjhb.site/Files.php/Books/(Uncategorized)/General%20Topology-John%20L.Kelley.pdf

Morris, Topology without Tears https://www.topologywithouttears.net/topbook.pdf

Lynn Arthur Steen & J. Arthur Seebach, Counterexamples in Topology, https://editorialdinosaurio.wordpress.com/wp-content/uploads/2012/03/counterexamples_in_topology_-_l-_steen__j-_seebach__1970__ww.pdf

Viro, Elementary Topology Problem Textbook https://www.maths.ed.ac.uk/~v1ranick/papers/viro.pdf

Matsumura, Introduction to Topology [lecture-notes] https://pi.math.cornell.edu/~matsumura/math4530/IntroToTopology.pdf

Renzo, Introduction to Topology [lecture-notes] https://www.math.colostate.edu/~renzo/teaching/Topology10/Notes.pdf

Warner, Topological Rings https://mezbanhabibi.ir/wp-content/uploads/2020/01/Topological-Rings-Warner.pdf

Simmons, Introduction to Topology and Modern Analysis https://github.com/anishLearnsToCode/books/blob/master/topology/Introduction-to-Topology-and-Modern-Analysis.pdf

## Algebra

Artin, Algebra https://media.githubusercontent.com/media/storagelfs/books/main/Applied%20Mathematics/Algebra/Artin.%20Algebra.%201991.pdf Solutions https://github.com/awasthi/math-solutions/blob/master/Artin/Artin%20Solutions.tex

Paolo Aluffi, Algebra: Chapter 0 https://agorism.dev/book/math/alg/algebra_chapter-0_paolo-aluffi.pdf

Charles C. Pinter, A Book of Abstract Algebra https://math.umd.edu/~jcohen/402/Pinter%20Algebra.pdf

Joseph A. Gallian, Contemporary Abstract Algebra https://github.com/dtbinh/OpenCourse/blob/master/AbstractAlgebra/Contemporary%20Abstract%20Algebra%209th%20Joseph%20A.%20Gallian.pdf

David S. Dummit & Richard M. Foote, Abstract Algebra https://www.gregkikola.com/dl/guides/dfsol.pdf

I.N. Herstein, Topics in Algebra http://www.uop.edu.pk/ocontents/Topics%20in%20Algebra%20by%20I.%20N.%20Herstein.pdf

Serge Lang, Algebra https://eclass.upatras.gr/modules/document/file.php/MATH1229/Algebra%20by%20Serge%20Lang%20%28z-lib.org%29.pdf

Nathan Jacobson, Basic Algebra https://www.math.toronto.edu/~ila/Jacobson-Basic_algebra_I%20(1).pdf

Thomas W. Hungerford, Algebra https://pages.cs.wisc.edu/~dluu/ps/Wilson's%20solutions%20to%20Hungerford%20-%20Algebra.pdf

Joseph J. Rotman, An Introduction to the Theory of Groups https://eclass.uoa.gr/modules/document/file.php/MATH784/Rotman%20An%20introduction%20to%20the%20theory%20of%20groups%20%281%29.pdf







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

