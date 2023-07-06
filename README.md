## **Inverse Transform** <br>

<Details>
<Summary> <i>Tools:</i> </Summary>

##### Actions:  [![Repo-Visualization-Badge](https://img.shields.io/badge/Action-Visualization-020521?style=square&logo=github&logoColor=white)](https://githubnext.com/projects/repo-visualization)
##### Main Text-Editor:  [![VSCode-Badge](https://img.shields.io/badge/VSCode-007ACC?style=square&logo=visual-studio-code&logoColor=white)](https://code.visualstudio.com/)  [![Jupyter-Badge](https://img.shields.io/badge/Jupyter-F37626?style=square&logo=Jupyter&logoColor=white)](https://jupyter.org/try)
##### Language:  [![Python-Badge](https://img.shields.io/badge/Python-2b6dd6.svg?style=square&logo=Python&logoColor=green)](https://www.python.org)[![Markdown-Badge](https://img.shields.io/badge/Markdown-000000.svg?style=square&logo=Markdown&logoColor=white)](https://www.markdownguide.org)[![yaml-Badge](https://img.shields.io/badge/YAML-000000?style=square&logo=yaml&logoColor=red)](https://yaml.org)  [![LaTeX-Badge](https://img.shields.io/badge/LaTeX-white.svg?style=flat-square&logo=LaTeX&logoColor=008080)](https://www.latex-project.org)
##### Libraries:  [![Numpy-Badge](https://img.shields.io/badge/Numpy-013243?style=square&logo=numpy&logoColor=white)](https://numpy.org)  [![Matplotlib-Badge](https://img.shields.io/badge/Matplotlib-40403f?style=square&logo=python&logoColor=blue)](https://matplotlib.org)  [![Random-Badge](https://img.shields.io/badge/Math-000000?style=square&logo=python&logoColor=white)](https://docs.python.org/3/library/random.html)
##### Interface:  [![React-Badge](https://img.shields.io/badge/React-61DAFB?style=square&logo=react&logoColor=black)](https://create-react-app.dev)
##### Version Control:  [![GitHub-Badge](https://img.shields.io/badge/GitHub-100000?style=square&logo=github&logoColor=white)](https://github.com)  [![Git-Badge](https://img.shields.io/badge/Git-F05032.svg?style=square&logo=Git&logoColor=white)](https://git-scm.com)
[![Git-Commads](https://img.shields.io/badge/Git%20Commands-gray?style=square&logo=git&logoColor=white)](https://github.com/EstebanMqz/Git-Commands)
##### License:&nbsp;[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

</Details>


<Details>
<Summary> <i>Contact:</i> </Summary>

[![Website](https://img.shields.io/badge/Website-ffffff?style=square&logo=opera&logoColor=red)](https://estebanmqz.com) [![LinkedIn](https://img.shields.io/badge/LinkedIn-041a80?style=square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/esteban-m65381722210212839/) [![Portfolio](https://img.shields.io/badge/Github-Portfolio-010b38?style=square&logo=github&logoColor=black)](https://estebanmqz.github.io/Portfolio/) [![E-mail](https://img.shields.io/badge/Business-Mail-052ce6?style=square&logo=mail&logoColor=white)](mailto:esteban@esteban.com)  

![GitHub Logo](https://github.com/EstebanMqz.png?size=25) [![Github](https://img.shields.io/badge/Github-000000?style=square&logo=github&logoColor=white)](https://github.com/EstebanMqz)
<br><br>


[MarcoSC08](https://github.com/MarcoSC08)

</Details>

<a name ="rpeo-visualization"></a>

<Details> <Summary> <i> Repository Visualization: </i> </Summary>
  
[![Repository](https://img.shields.io/badge/Repository-0089D6?style=square&logo=microsoft-azure&logoColor=white)](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=EstebanMqz%2FInverse-Transform) [![Jupyter](https://img.shields.io/badge/Render-nbviewer-000000?style=square&logo=jupyter&logoColor=orange)](https://nbviewer.org/github/EstebanMqz/Inverse-Transform/blob/main/Inverse-Transform.ipynb)


<img src="diagram.svg" width="280" height="280">

</Details>

<br>

<b>Description:</b>

[Github-app parse](https://github.com/EstebanMqz/Inverse-Transform/blob/main/images/Description.jpg)

In this repository the [**Inverse-transform**](README.md#references) sampling method is illustrated with:

1. $X~\sim U(a, b)$ for [***uniformly distributed***](README.md#references) <u>continuous</u> random variables:

[*`PDF`*](https://en.wikipedia.org/wiki/Probability_density_function) $\rightarrow$ $f(x)$  = $\frac{1}{b-a}$

$$F(x) = \int_{-\infty}^{x} f(x) dx = \int_{a}^{x} \frac{1}{b-a} dx = {\frac{x}{b-a}} \Big|_{a}^{x} = \frac{x-a}{b-a}$$ 

<br><br>

$\therefore$ The Inverse Transform [*`CDF`*](https://en.wikipedia.org/wiki/Cumulative_distribution_function) $\rightarrow F(X)$ [*pseudo-random number samplings*](README.md#references) $X_i \in [a, b]$ is: 

$$U = F^{-1}(X) = x(b-a) + a$$ 
<br>

2. $X~\sim B(k; n, p)$ <u>discrete</u> [***Binomial distribution***](README.md#references):<br>

If the probability $p$ of $k$ successes in $n$ trials is given by $X = 10000$ samplings.

$$Pr(k;n,p) = Pr(X=k;n,p) = \binom{n}{k} p^k (1-p)^{n-k}$$

where 

$$\binom{n}{k} = \frac{n!}{k!(n-k)!}$$

Expressed with factorial operations as:

$$Pr(k;n,p) = \frac{n!}{k!(n-k)!} p^k (1-p)^{n-k}$$

$\therefore$ $k + 1$ $\times$ the ratio of trials to successes is: 

$$Pr(k+1;n,p) = \frac{(n-k) p}{(k+1)(1-p)} Pr(k;n,p)$$

Analytical results with the further use of [`numpy.random.random`](README.md#references) & [`numpy.random.binomial`](README.md#references) validated with matplot<br>
*(see repo-visualization → nbviewer)*

<br>

###### References:

<a name ="References"></a>

+ [Binomial distribution](https://en.wikipedia.org/wiki/Binomial_distribution)<br>
+ [Uniform distribution](https://en.wikipedia.org/wiki/Continuous_uniform_distribution#Related_distributions)<br>
+ [Inverse Transform samplings](https://en.wikipedia.org/wiki/Inverse_transform_sampling)<br>
+ [<i>Pseudo-random number samplings</i>](https://en.wikipedia.org/wiki/Non-uniform_random_variate_generation#:~:text=Non-uniform%20random%20variate%20generation%20or%20pseudo-random%20number%20sampling,a%20uniformly%20distributed%20PRN%20generator.)<br>
+ [<b>(PDF)</b> <i> Probability density function </i>](https://en.wikipedia.org/wiki/Probability_density_function)<br>
+ [<b>(CDF)</b> <i> Cumulative density function </i>](https://en.wikipedia.org/wiki/Cumulative_distribution_function)<br>
+ [`numpy.random.random`](https://numpy.org/doc/stable/reference/random/generated/numpy.random.random.html) [`numpy.random.rand`](https://numpy.org/doc/stable/reference/random/generated/numpy.random.rand.html)  
+ [`numpy.random.binomial`](https://numpy.org/doc/stable/reference/random/generated/numpy.random.binomial.html)<br>
+ [LaTeX](https://en.wikipedia.org/wiki/List_of_mathematical_symbols_by_subject)<br>
