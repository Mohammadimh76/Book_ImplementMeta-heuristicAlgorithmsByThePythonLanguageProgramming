## "Implement  Meta-heuristic algorithms by the Python language programming" 🔺(Coming Soon)🔺


---

## Introduction:
In recent years, the use of meta-heuristic algorithms has expanded significantly in solving complex computational problems, and today it has many applications in various branches of science. They may be close to the global optimum.<br>
The present book is an attempt to present the concepts of meta-heuristic algorithms, their implementation and applications, consisting of 6 main chapters and two comprehensive appendices. The first chapter of the book contains an overview of optimization methods and familiarity with the components and classification of different types of optimization problems. Chapters 2 through 6 cover refrigeration simulation algorithms, forbidden search, genetic algorithms, ant colony optimization, and particle mass optimization. Appendix (a) also includes a step-by-step tutorial on Python software that students will gain the necessary mastery of Python software by reading and practicing this chapter. Appendix (b) also provides programming related to widely used algorithms.<br>
It is hoped that this small effort will be used by respected scholars and will improve their scientific level. We ask all the dear readers to help the authors of the book in eliminating the shortcomings and improving the presented materials by sending their constructive suggestions and criticisms.<br>
Authors Group


| Front Book Cover  | Back Book Cover  |
|-----------|--------------------|
|<p><img src="https://raw.githubusercontent.com/Mohammadimh76/Mohammadimh76.github.io/master/Book_7.jpeg"></p>|<p><img src="https://raw.githubusercontent.com/Mohammadimh76/Mohammadimh76.github.io/master/Book_7_b.jpeg"></p>|
|  <b>Book Name</b>   |   Implement  Meta-heuristic algorithms by the Python language programming  |
| <b>Authors</b>    |   M.H.Mohammadi, A.Karimi|
| <b>language</b>    |  <b>English</b>   |
| <b>Printed in the</b>    |  ...   |
| <b>Publisher</b>    |   ...  |
| <b>First Printing Edition</b>    |   🔺<b>Coming Soon</b>  |
| <b>Print Length</b>    |  ...   |
| <b>ISBN</b>    |  0-0000000-0-0   |

---

## Contents:

- <b>Chapter (1):</b> Optimization methods
- <b>Chapter (2):</b> Simulated Annealing (SA) 
- <b>Chapter (3):</b> Tabu Search (TS)
- <b>Chapter (4):</b> Genetic Algorithm (GA)
- <b>Chapter (5):</b> Ant Colony Optimization algorithms (ACO)
- <b>Chapter (6):</b> Particle Swarm Optimization (PSO)

| <b>Chapter 1</b>  | <b>Chapter 2</b>  |<b>Chapter 3</b>  |
|-----------|--------------------|--------------------
| 1-1- Introduction |2-1- Introduction |3-1- Introduction|
| 1-2- Basic components of optimization problems | 2-2- Simulated Annealing         | 3-2- The concept of using memory in search is forbidden |
| 1-3- Classification of optimization problems | 2-3- Optimal localized points | 3-3- Basic parameters in the forbidden search method |
| 1-4- Types of optimization solutions | 2-4- Mapping the concepts of the cooling process as an optimization problem | 3-4- Fundamentals of Forbidden Search Approach |
| 1-5- Classification of optimization methods | 2-5- Mathematical concept of refrigeration simulation | 3-5- Applications |
| | 2-6- Refrigeration simulation algorithm implementation process | |
| | 2-7- Modified versions of the refrigeration simulation algorithm  | |
| | 2-8- Advantages and disadvantages of refrigeration simulation algorithm | |
| | 2-9- Comparison of refrigeration simulation algorithm with genetic algorithm | |
| | 2-10- Applications of refrigeration simulation algorithm  | |


| <b>Chapter 4</b>  | <b>Chapter 5</b>  |<b>Chapter 6</b>  |
|-----------|--------------------|--------------------
| 4-1- Introduction| 5-1- Introduction  | 6-1- Introduction   |
| 4-2- The concept of evolution | 5-2- Ant Colony Optimization algorithms | 6-2- Collective intelligence |
| 4-3- An overview of natural genetics | 5-3- The ants algorithm for the itinerant vendor problem  | 6-3- Particle Swarm Optimization |
| 4-4- Genetic algorithm | 5-4- Some modified versions of the Ants algorithm | 6-4- Social network structures          |
| 4-5- Types of Genetic algorithms | 5-5- General parameters of ACO algorithm  | 6-5- Particle mass optimization parameters  |
| 4-6- A variety of genetic algorithm methods | 5-6- Differences in ant colony optimization with other collective intelligence algorithms | 6-6- The effect of quantification on particle mass optimization parameters  |
| 4-7- Genetic algorithm capabilities | 5-7- Applications  | 6-7- Combined algorithms  |
| 4-8- Disadvantages of genetic algorithms | | 6-8- Optimization of issues with constraints  |
| 4-9- Applications | | 6-9- Disadvantages of particle mass optimization algorithm  |
| |  | 6-10- Applications          |





## Chapter (1) - Optimization methods
There are search methods that aim to find an answer to the optimization problem, so that the quantity under consideration is optimized, although some more complex issues are not considered in this definition. For example, the answer could be a combination of Include different types of data, limit non-linear search space, specify problem over time, or quantities to be optimized for conflicting purposes. These are just a few small examples of the complexities of an optimization algorithm, and are briefly reviewed in this chapter. 

## Chapter (2) - Simulated Annealing (SA) 
Optimization is the process that is followed to make something better. The idea, idea or design put forward by a scientist or engineer gets better during the optimization process. During optimization, the initial conditions are examined in different ways and the information obtained is used to improve an idea or method. Optimization is a mathematical tool used to find answers to many questions about how to solve various problems.<br>
Optimization refers to finding the best answer to a problem. The word best implicitly states that there is more than one answer to a problem that is not of equal value. Defining the best answer to the problem under consideration is the method of solving And also the amount of error allowed depends; Therefore, how the problem is formulated also has a direct impact on how the best answer is defined. Some questioners have definite answers. The best player in a sport, the longest day of the year, and the answer to a typical first-order differential equation are examples of simple problems.<br>

<p align="center">
  <img width="420" height="237" src="https://github.com/Mohammadimh76/Book_ImplementMeta-heuristicAlgorithmsByThePythonLanguageProgramming/blob/main/Gif/SimulatedAnnealing.gif">
</p>

In contrast, some problems have multiple maximum or minimum answers, known as optimal or extreme points, and the best answer is probably a relative concept. The best works of art, the most beautiful scenery and the most pleasing piece of music are some of the examples that can be given for such issues.<br>
In mathematics, there are beautiful ways to solve the optimization problem. These methods are valid and easy to use for some cost functions. Many complex problems can be transformed into functions with a little change and analysis, which can be found to be the minimum or maximum value using analytical methods.<br>
The extreme points of any function are the first-order derivatives of that function. In this way, by deriving the function and setting its value to zero and solving the resulting equation, the location of the extreme points can be obtained. If the sign of the second derivative of the function is negative at an extreme point, the obtained extreme point is a local minimum point for the function under consideration. Similarly, the positive sign for the second derivative indicates the existence of a local maximum point. Scalar is valid. For multivariate functions, the equations defined in the vector differential calculus can be used.<br>
For example, a function gradient is used instead of a derivative. Many methods have been proposed to improve the analytical optimization process, but in general, for problems that are complex or do not have a clear mathematical definition, the analytical method assumes efficiency. It will not have.<br>

<p align="center">
  <img width="420" height="315" src="https://github.com/Mohammadimh76/Book_ImplementMeta-heuristicAlgorithmsByThePythonLanguageProgramming/blob/main/Gif/SimulatedAnnealing_2.gif">
</p>

In contrast, there are methods that are inspired by nature and do not have a specific function, but the behavior of these algorithms is mostly described by random quantities. It should be noted that in our opinion, the behavior of nature is unpredictable and therefore methods We have modeled nature attributes with random numbers, but this attitude is most likely due to our lack of understanding of nature's behavior. Nature-derived methods, in addition to their many beauties, also bring us the power of nature. Nature is always optimizing and some people believe that it always does the best it can. Nature-inspired methods are in fact conscious imitations of nature to use a nature-like method in dealing with various issues. One of the algorithms that falls into this category is the refrigeration simulation algorithm or the open algorithm. Baking (SA) is the subject of discussion and will be explained below. 

## Chapter (3) - Tabu Search (TS)
Given the challenges of solving complex optimization problems in the real world, classical methods often face many problems. Important and essential applications in business, engineering, economics, and science using methods that have focused primarily on academic research for the past three decades cannot be reasonably hoped for success. In contrast, meta-innovative approaches have dramatically altered our ability to solve business, applied science, and engineering problems. Many of these methods use a local search mechanism, which is an iterative search process that starts with a solvable search and searches in the solution space to reach a local optimization. continues. Since the quality of the answer obtained in a local search is largely dependent on the movements defined, this local optimization will usually be nothing more than an average answer. This is a major problem in local search-based approaches.<br>
Glover (م introduced the Forbidden Search Method (TS) method 1986 in 1986 to address the shortcomings associated with local search algorithms, which is based on the direct obstruction of the search algorithm from accessing difficult areas of the solution space. Different forms such as prohibition of type navigation in the solution space, prohibition of one or more areas of the solution space from the search process. This method is based on the selection of concepts from the fields of artificial intelligence and optimization and the local search method. Leads to a search for space farther from the local optimization, and in this way the creation of adaptable memory has dramatically increased our ability to solve a variety of problems, including recent responses or movements. In fact, the forbidden search algorithm can be considered as a combination of a short-term memory and a local search mechanism.<br>

<p align="center">
  <img width="450" height="253" src="https://github.com/Mohammadimh76/Book_ImplementMeta-heuristicAlgorithmsByThePythonLanguageProgramming/blob/main/Gif/TabuSearch.gif">
</p>

The word ta bo comes from a Polynesian language, used in the past by the indigenous peoples of Tonga to forbid sacred objects that should not be touched. According to the Webster Dictionary, the word now means "prohibition imposed by society. In the form of a "preventive measure" or "prohibited due to danger". The latter meaning, that is, prohibition due to danger, is very much in line with the subject of taboo search. Just as in society, "preventive prohibition" can be replaced by other things if necessary, prohibited search taboos can be revised when there are desirable alternatives.

## Chapter (4) - Genetic Algorithm (GA)
Genetic Algorithm (GA) is an optimization and search algorithm based on the principles of genetics and natural selection. In a genetic algorithm, a group of individuals emerge and develop in a situation where the overall goal is to maximize the merits of the entire population or minimize a population-related cost. John Holland introduced the method in the 1960s and 1970s, but it was eventually put together by one of his students, David Goldberg. Holland's early work was collected, published and published in his book. He was the first to attempt to provide a theoretical basis for genetic algorithms by articulating pattern theory. The results of Diong's study, published in 1977, showed that the genetic algorithm was effective in optimizing functions. He took the first organized action to find the optimal value of the parameters of the genetic algorithm. In general, Goldberg has the largest share in the development of genetic algorithms; Because he offered many successful applications for genetic algorithms and wrote a very useful book about it. Since then, many evolutionary algorithms have been proposed and developed for various applications (Randy et al., 2004; Mitchell Melanie, 1999; Amit Connar, 2000; Goldberg,1989).<br>
As mentioned, the genetic algorithm is one of the most important innovative algorithms used to optimize various functions and was first proposed by John Holland at the University of Michigan. In this algorithm, past information - due to heredity - is extracted and used in the search process. , Are random search techniques that are based on natural selection and natural genealogy. These algorithms are fundamentally different from conventional search and optimization methods, as Goldberg summarizes them.<br>

- The genetic algorithm works with encoded sets, not with them
- The genetic algorithm starts the search process with a set of answers, not just one
- The genetic algorithm uses fitting function information, not other derivatives or auxiliary methods
- The genetic algorithm uses probabilistic rules, not definite rules

In this chapter, first a list of basic concepts about genetic algorithm is presented and then the constituent elements of genetic algorithm are introduced.

## Chapter (5) - Ant Colony Optimization algorithms (ACO)
Ants appeared on Earth about a hundred million years ago. These insects have a social life with collective behaviors. Although only 2% of insect species have social life, ants make up more than 50% of the insect biomass. In some places, such as the Amazon rainforest, the rate rises to more than 4 percent. Social life means the accumulation of a large number of a particular species in the form of a collection or colony and their interaction with each other. All ants and termites, as well as some species of bees, live in colonies. Insect communities can work together to resolve issues that none of the members of that community alone can solve. Most of these problems can be expressed in terms of optimization. Babies are one of the optimization problems that social insects solve together. These problems all have equivalents among everyday optimization problems (Olario and Zumaya, 2006; Sayari et al., 2006; Dorigo et al., 2006; Dorigo and Di Caro, p. 1999).<br>

## Chapter (6) - Particle Swarm Optimization (PSO)
### 🔺(Coming Soon)🔺


---

## Authors

### The First: "Mohammad Hossein Mohammadi"

<p align="center">
  <img width="360" height="276" src="https://raw.githubusercontent.com/Mohammadimh76/Book_MetaheuristicWithPython/main/Authors/MohammadHosseinMohammadi.jpeg">
</p>

Iam currently a Final-year BS.c student at the Department of Computer Engineering, Islamic Azad University, Najafabad Branch (IAUN) (Rank in CWUR) where I am a member of the Bioinformatics Laboratory (BL), advised by Prof. Mohammad Naderi Dehkordi. my research involves machine vision, deep learning, and neural networks. where I will complete my thesis on Accurate and Early Identification of Diabetes and it's Affecting Factors.

Prior to BL, I finished my Diploma - Mathematics and Physics in Sheikh Ansari Highschool, in September 2015. I tried to use my Diploma to build a solid bedrock for my future research. So in addition to taking many optional bachelor-level courses on math and computer science. I spent 6 months as an intern Programmer at the "CoTech" in Isfahan.

#### My main research interests
- Artificial Intelligence, Machine Learning
- Optimization Algorithm, Neural & NeuroFuzzy Network
- Computer Vision, Signal and Image Processing

🌐 𝐏𝐞𝐫𝐬𝐨𝐧𝐚𝐥 𝐏𝐚𝐠𝐞 "𝐌𝐨𝐡𝐚𝐦𝐦𝐚𝐝 𝐇𝐨𝐬𝐬𝐞𝐢𝐧 𝐌𝐨𝐡𝐚𝐦𝐦𝐚𝐝𝐢" 👉 [mohammadimh76.github.io](https://mohammadimh76.github.io/)<br>
📧 𝐄𝐦𝐚𝐢𝐥: m.h.mohammadimir2017@gmail.com

============================================================================

### The Second: "Ali Karimi"

<p align="center">
  <img width="320" height="320" src="https://raw.githubusercontent.com/Mohammadimh76/Book_MetaheuristicWithPython/main/Authors/AliKarimi.jpeg">
</p>

Iam currently a second-year MS.c student at the Department of Electrical and Computer Engineering, University of Tehran (UT) where I am a member of the Multimedia Processing Laboratory (MPL), advised by Prof. Mohammad Ghanbari. my research involves machine vision, deep learning, and neural networks.

Prior to MPL, I finished my BSc in Computer Engineering at the Department of Computer Engineering, Bu-Ali Sina University, in August 2018. I tried to use my bachelor's to build a solid bedrock for my future research. So in addition to taking many optional graduate-level courses on math and computer science. I spent a year as a Research Assistant at the Computer Networks Laboratory at the Bu-Ali Sina University where I completed my thesis on Evaluating and Improving the LoRa Protocol performance.

🌐 𝐏𝐞𝐫𝐬𝐨𝐧𝐚𝐥 𝐏𝐚𝐠𝐞 "𝐀𝐥𝐢 𝐊𝐚𝐫𝐢𝐦𝐢" 👉 [alikarimi120.github.io](https://alikarimi120.github.io/)<br>
📧 𝐄𝐦𝐚𝐢𝐥: alikarimi120@gmail.com 


---
---

👇Click on the link below to see the E-Book Demo!👇😉

## (E-Book Demo): 🔺(Coming Soon)🔺



