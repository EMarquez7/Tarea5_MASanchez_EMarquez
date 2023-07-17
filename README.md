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

<a name ="repo-visualization"></a>

<Details> <Summary> <i> Repository Visualization: </i> </Summary>
  
[![Repository](https://img.shields.io/badge/Repository-0089D6?style=square&logo=microsoft-azure&logoColor=white)](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=EstebanMqz%2FInverse-Transform) [![Jupyter](https://img.shields.io/badge/Render-nbviewer-000000?style=square&logo=jupyter&logoColor=orange)](https://nbviewer.org/github/EstebanMqz/Inverse-Transform/blob/main/Inverse-Transform.ipynb)


<img src="diagram.svg" width="280" height="280">

</Details>


<div align="right">
<Details>
<Summary> <i>Contact:</i> </Summary>
  
[![Website](https://img.shields.io/badge/Website-ffffff?style=square&logo=opera&logoColor=red)](https://estebanmqz.com) [![LinkedIn](https://img.shields.io/badge/LinkedIn-041a80?style=square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/esteban-m65381722210212839/) [![Portfolio](https://img.shields.io/badge/Github-Portfolio-010b38?style=square&logo=github&logoColor=black)](https://estebanmqz.github.io/Portfolio/) [![E-mail](https://img.shields.io/badge/Business-Mail-052ce6?style=square&logo=mail&logoColor=white)](mailto:esteban@esteban.com)

![GitHub Logo](https://github.com/EstebanMqz.png?size=50) [![Github](https://img.shields.io/badge/Github-000000?style=square&logo=github&logoColor=white)](https://github.com/EstebanMqz)


[MarcoSC08](https://github.com/MarcoSC08)

</Details></div>

---

<Details> <Summary> <b> Description: </b> </Summary>
  
<br>

[Github-app parse](https://github.com/EstebanMqz/Inverse-Transform/blob/main/images/Description.jpg)

In this repository the [**Inverse-transform**](README.md#references) method is illustrated with $n=10000$ samplings for the following:

<b>1.</b> [*`CDF`*](README.md#References) $\rightarrow$ $F(x)$  = $\frac{2}{\pi}\sin^{-1}(\sqrt x)$

$$U = F^{-1}(X) = \sin^{2}(\frac{\pi}{2}X)$$

where $X~\sim U(a, b)$ is [***uniformly distributed***](README.md#references) by definition. 

<b>2.</b> [***Binomial distribution***](README.md#references) (<i>discrete</i>) with a [*`PMF`*](README.md#References) $X \sim B(X=k; n, p)$.

$$Pr(X=k;n,p) = \binom{n}{k} p^k (1-p)^{n-k}$$

where the binomial coefficient combinatorial of $k$ sucesses possible in $n$ trials $_n C_k$ can be expressed as:
$$_n C_k = \frac{n!}{k!(n-k)!}$$

And generalized to the $k + 1$ $\times$ $\frac{p}{1-p}$ ratio:

$$Pr(k+1;n,p) = \frac{n!}{(k+1)(k)!(n-k-1)!} p^{k+1} (1-p)^{n-k-1}$$

$$Pr(k+1;n,p) = \frac{n-k}{(k+1)(1-p)} p^{k+1} (1-p)^{n-k-1}$$

$$Pr(k+1;n,p) = \frac{n-k}{(k+1)(1-p)} p (p^k (1-p)^{n-k})$$

$\therefore$ the $p$ prob. of $k$ sucesses in $n$ trials $\times$ their ratio is:

$$Pr(k+1;n,p) = \frac{(n-k) p}{(k+1)(1-p)} Pr(k;n,p)$$

<i>Samplings made with [`numpy.random.random`](README.md#references) & [`numpy.random.binomial`](README.md#references), validated with `matplotlib`.</i><br>

</Details>

<Details> <Summary> <b> Results: </b> </Summary>

<br>

As it can be seen in from $F(x)$ samplings, some density functions [`pdf`](README.md#references) have a probability $f(x)$ which is more likely to be modelled with its cumulative function [`cdf`](README.md#references). The inverse transform can be used for the generation of random variables in $x_i\in[0,1]$. 

$F(x)$  = $\frac{2}{\pi}\sin^{-1}(\sqrt x)$<br>


![Sin-Wave](https://github.com/EstebanMqz/Inverse-Transform/blob/main/images/Sin.jpg)

<br>

$X \sim B(X=k; n, p)$<br>

![Binomial](https://github.com/EstebanMqz/Inverse-Transform/blob/main/images/X~B(X%3Dk%3Bn%2C%20p).jpg)

</Details>

###### References:

<a name ="References"></a>

+ [Binomial distribution](https://en.wikipedia.org/wiki/Binomial_distribution)<br>
+ [Uniform distribution](https://en.wikipedia.org/wiki/Continuous_uniform_distribution#Related_distributions)<br>
+ [Inverse Transform samplings](https://en.wikipedia.org/wiki/Inverse_transform_sampling)<br>
+ [<b>(PDF)</b> <i> Probability density function </i>](https://en.wikipedia.org/wiki/Probability_density_function)<br>
+ [<b>(PMF)</b> <i> Probability mass function </i>](https://en.wikipedia.org/wiki/Probability_mass_function)<br>
+ [<b>(CDF)</b> <i> Cumulative density function </i>](https://en.wikipedia.org/wiki/Cumulative_distribution_function)<br>
+ [`numpy.random.random`](https://numpy.org/doc/stable/reference/random/generated/numpy.random.random.html) [`numpy.random.rand`](https://numpy.org/doc/stable/reference/random/generated/numpy.random.rand.html)  
+ [`numpy.random.binomial`](https://numpy.org/doc/stable/reference/random/generated/numpy.random.binomial.html)<br>
+ [LaTeX](https://en.wikipedia.org/wiki/List_of_mathematical_symbols_by_subject)<br>
