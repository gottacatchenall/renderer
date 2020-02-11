# Critical Transitions in Landscape Connectivity

_M.D. Catchen_, _S.M. Flaxman_

_Philosophers have hitherto only interpreted the world in various ways; the point is to change it._
Karl Marx, _Theses on Feuerbach (1845)_

## Abstract

this is where the abstract goes

\pagebreak  

## Introduction

Understanding how emergence of complex systems occurs is a problem  scale  

Human activity has, in a (geologically speaking) relatively short period of time, rapidly altered the face of the planet Earth. This drastic change in the structure of Earth's terrain has had overwhelmingly negative effects on the planet's biodiversity. Historically, the effect of land-use change on biodiversity has been studied under the banner of 'habitat fragmentation'. Much debate occured regarding what precisely is meant by this term---however what remains clear is that habitat loss is one of the leading drivers of biodiversity loss globally (cite).  

Ecological processes occur in space. 

Examples:

 - Habitat loss is a major threat to biodiversity.

 - Biogeography

 - Allopatric and Peripartic Speciation 

Landscape connectivity as fundemental to many questions. Practically, land use management and landscape 'design' are major methods for conserving biodiversity in face of cliamte change and continued hman development 

What needs to be done? 

What did I do, and why does it address what needs to be done?

\pagebreak

## Methods

### Ecological Dynamics on Spatial Graphs

Ecological data, especially data about biotic processes, is often pointlike—a measurement taken of some ecological process associated with a spatial coordinate. 

Spatial graphs are often used to model a system of habitat patches.

Here we model a system of populations, represented as nodes in a spatial graph, with edges representing dispersal between populations. We consider then consider a measurement of an ecological process at each site $f(x_i)$, which maps spatial locations to measurement values $f : \mathbb{R}  \to \mathbb{R}$.

In this paper, we consider the measurement in question to be the size of the population at that point.

Here we propose modeling landscape connectivity as a combination of two different factors: the probability than any individual migrates during its lifetime, $P(m)$, and the conditional distribution of where an individual migrates to given where they started, often called the dispersal kernel. For example, if we denote the probability that an individual born in $X_i$ reproduces in $X_j$ as $P(X_j | X_i)$, we can define the dispersal matrix as

$$\Phi_{ij}= \begin{cases} P(X_j | X_i)\ P(m)   &\quad\text{if} \  i \neq j \\ 1 - P(m)  &\quad\text{if}\ i = j\end{cases}   $$

Here $\Phi_{ij}$ represents the probability that any individual born in $i$ reproduces in $j$.

We then can consider modeling the dispersal kernel, $P(X_j | X_i )$ , using a variety of methods. This is in

Empirically, resistance surfaces are a good way to model this. Theoretically, various functional forms representing isolation-by-distance have been used. (See next section).

Now we move to considering the dynamics an ecological process/measurement taken at each site, $f(x_i)$. We can now represent the dynamics of this system using a reaction-diffusion model,

hey fartbag you have to explain why matrix notation works $\dot{x_i} = (1-m)x_i + m \sum_{j \neq i} \Phi_{ji} x_j$

$$\frac{d\vec{x}}{dt}= g(\Phi^T \vec{x})$$ 

Here, $g(x)$ is a function that represents the hypothesized mechanism that represents how the ecological measurement evolves locally. For example, in the next section we will consider the stochastic logistic model, $$g(x) = \lambda x(k-x) + \sigma dW$$ 

However, $g(x)$ can represent any ecological process of interest, for example if the state space of $x$ is allelic frequencies, $g(x)$ could describe genetic drift, or if $x$ represents community compositions across space, $g(x)$ could describe competition between species as a function of environmental conditions. Coevolutionary states across space, mosaic, etc.  

### Transitions in the Synchrony of Metapopulation Dynamics

Here, we apply the above SGD framework to answer the question: when do transitions from the system behaving as one unified system to many independent systems occur?

One can intuitively assess the boundary conditions of this problem: if the probability that any individual migrates $P(m) =  0$, the system is not one but instead a collection of independent systems. However, if $P(m)=1$, the spatial structure ceases to carry much meaning and the system is one unified system. Where in the space of landscape connectivity, as represented by $\Phi$, does a system of metapopulation dynamics shift from being several independent populations to one single population? 

#### Population Dynamics

We model population dynamics within each local population $X_i$ using the stochastic logistic model. The dynamics of the number of individuals in population i are described by the stochastic differential equation   

$$dN_i = K_{i} \lambda_i (K_i-N_i) dt + \sigma dW$$

For the sake of reducing parameter space, we consider all populations as having the same $\lambda_i$ and $K_i$, however, future work could include exploring the source-sink dynamics in this system by varying intrinsic growth rates and carrying capacities across populations. 

#### Measuring Synchrony

We must first determine what we mean when we say that a metapopulation is a single, unified system versus many indepedent systems. In the context of population dynamics, we consider the total sum of the count of individuals across all sites as $N(t)$  
$$N(t) = \sum_i N_i(t)$$

If the dynamics of two systems are independent, then we would expect weak  correlation between $\Delta =N(t+1) - N(t)$ and $\Delta_i=N_i(t+1) - N_i(t)$.
However, if the system is truly ‘one’, then we would expect iand jto be the same. 
The crosscorrelation between two vectors $\vec{X}$ and $\vec{Y}$ is given by 

$$R_{XY} = \begin{bmatrix} E[X_1Y_1] & E[X_1Y_2] & \dots \\ E[X_2Y_1] & E[X_2Y_2] & \dots \\  \vdots & \vdots & \ddots  \end{bmatrix}$$

Luckily, there is already a variety of tools used to measure correlations between time-series. Crosscorrelation function, lags, etc.

### Numerical Simulations

Optimizing a landscape numerically

How do you maximize synchrony based on limited amount of possible change dispersal potential space?

evenness of eigenvalue centrality compared to numerical computation over whole space

## Results

In figure one we can see

## Discussion

landscape connectivity is a function of scale.

## References