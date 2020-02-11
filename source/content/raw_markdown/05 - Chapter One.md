# Simulation Models in Ecology 

_M.D. Catchen_, _S.M. Flaxman_ 

\pagenumbering{arabic}  

> _The electron is a theory we use; it is so useful in understanding the way nature works that we can almost call it real._

> _Richard P. Feynman_

> The limits of language means the limits of my world.*   

> Ludwig Wittgenstein (1922)

> Things are similar: this makes science possible. Things are different: this makes science necessary.

>Levins & Lewontin (1985)

## Abstract

this is where the abstract goes

## Introduction

### What is science?

Science is functionally a theory of epistemology—a way of knowing. Scientific knowledge takes the form of theories—explanations of natural phenomena. Within scientific epistemology, for a theory to be scientific, it must be capable of being disproven through observation, meaning it must make predictions that may or may not agree with observed reality.

So, a valid scientific theory must make predictions that can be observed, and therefore must account for some measurable state of the universe.

Theories must be embodied in language. One subtle consequence of this is that there is a limitation on what we can understand scientifically—that which we can represent in language @Wittgenstein. The limitations of what a language can represent, then, places a limit on what we can any given scientific theory can describe. In practice, the language of scientific theories can be split into: (conceptual, qualitative, English), (quantitative, math). Different languages have different costs and benefits when describing theories.

For example, if we wish to understand the properties of gravity, we are limited by the differences in what we can describe in diffent languages. For example, consider the following three theories:

$$T_1 : \text{bodies with mass exert an attractive force on one another} $$
$$ T_2: \quad F_G = \frac{Gm_1m_2}{r^2} $$
$$T_3: R_{\mu v} -\frac{1}{2} Rg_{\mu v} - \Lambda g_{\mu v} = \frac{8\pi G}{c^4}T_{\mu v}$$

What unites scientific theories across languages is that they all use constructed definitions. This is a necessary byproduct of being embodied in language. For example, for $T_1$ to convey information, one must first understand what is meant by 'bodies', 'mass', 'force', etc.  

All of them describe the same phenomena, and are, at least in some sense, correct (more on this in the next section). 

They also take input and output, must make a prediction.

Different languages differ in the precision of the predictions they can make.

Validation of a model: more parameters means more difficult to \*disprove.\*

Ratio between information described by the model and predictive capacity

### What makes a theory correct?
 _To know how to distinguish between true and false, one must have an adequate idea of true and false._
Baruch Spinoza, _Ethics_

All three theories are, in a sense, correct$^1$. 

 Why do we mean when we say a theory is accurate?  Notice that as our model increases in its predictive accuracy, it engages with more constructs. Not an act of discovery, but an act of creation. Is the Ricci tensor $g_{\mu v}$ real? It is a construct related to measurable quantities.

### What is a model?

The role of a theory in scientific epistemology is now what is often refered to as a 'model'.

Theories must be embodied in language. The limitations of the language you use to describe a theory places limitations on what you can describe (Wittgenstein). For example, Verbal explanation gravity vs Newton vs. General Relativity? Are all three right? Is rightness just predictive accuracy down to a degree of error?

@Cousteau1963

Theory / model as interchangeable words

For a theory to be scientific, must make predictions. Like a function: maps some input conditions to a predicted output. 

Much easier to describe the mechanism of interactions than to describe the dynamics that unfold from them. use computers to sample that.



### Why Simulate?

Stochasticity is ubiquitous in ecological processes.

The tools we have to handle analytic probability limits the coplexity of what we can consider.

Simulation allows us to describe the distribution of complex stochastic processes that cannot be easily explored with anlytical tools. 

Use computers to simulate to test mechanism, forecast, etc. Cite simulation as use 

Approximate Bayesian Computation, intractable liklihood

### Types of Models

high variance in predictions in ecology, complex mechanisms, stochasticity. tools of math makes it harder to validate predictions. no theory describes everything perfectly. even newton’s gravity becomes intractable w/ 3 body prob. 

Karl Popper, demarcation and falsifiable. Observation is not without theory. This collides with ecology. The model is always there, fish in water. 

Most theories of model selection revolve around information theoretic criteria 
Cartesian reductionism and emergent phenomena 
Simulation models for dealing with complex systems
   
Types of models:
  - data-models: 
    - process-based
      - naive toy models
      - ibm, etc. we got those parameters you asked for boss
     - stupid classic stats stuff
  - algorithmic models:
    - predictive, but with no way of assessing mechanism. overfitting 

Simulation models as a way of testing mechanism, computational power now available 

Habitat loss and fragmentation are the primary causes of anthropogenic extinctions, and pose significant threats to biodiversity and ecosystem health around the globe (Haddad et al. 2015, Rands et. al 2010, Fahrig 2003). As a result, the literature surrounding habitat fragmentation is vast and spans and wide variety of subfields, and a wide-variety of definitions are used to describe fragmentation. “Habitat fragmentation” is often used as a catchall to refer to one or more of  increasing patch-isolation, the loss of habitable matrix, and/or reductions in landscape connectivity. Fahrig (2003) defines fragmentation per se  as purely the separation/isolation of a fixed amount of habitat. In no small part due to ambiguous (and sometimes conflicting) definitions, a wide variety of conceptual approaches have been used to study fragmentation and its effects, ranging from focusing on the loss of patch area, the effects of landscape heterogeneity, disruption of interactions between species, edge-effects, and patch connectivity (Fischer and Lindenmayer 2007). 

Broadly speaking, the conceptual models of habitat fragmentation have their roots in one of two subfields: island biogeography and metapopulation ecology (Collinge 2009). The Theory of Island Biogeography (TIBG), introduced by MacArthur and Wilson (1967), was conceptualized for terrestrial communities on oceanic islands, but it quickly was applied elsewhere under the assumption that many human-altered landscapes are well-approximated by an island structure—isolated regions of homogeneous landscape separated by inhabitable matrix (Haila 2002). The core ideas of TIBG relate island sizes and distances from one another to species richness. These ideas thus led to focus on both the amount of habitat available, and the dispersal structure of the islands. Many of the theoretical studies in the 1980s and 1990s focused explicitly on the relationship between habitable area and species persistence, such as percolation theory, and extinction debt.  Haila (2002) critiques these assumptions and suggests re-conceptualizing fragmentation as a type of "human-induced environmental degradation". 

The second main subfield, the metapopulation framework, was introduced by Levins (1969), who modeled a system of infinitely many populations, each with a uniform probability of colonization or local extinction each generation. Metapopulation theory was more formally applied to fragmented landscapes by Hanski and Ovaskainen, who refined the Levins model to a finite number of populations with spatially-explicit locations, each with a unique probability of colonization arising from the metapopulation's spatial structure. Models of this form are called Incidence-Function Models (IFMs) (Hanski 1994; Hanski and Ovaskainen 2000). IFMs have seen extensive use in conservation (cite some papers that have used IFM).  Both the Levins model and IFMs are occupancy models: each patch/population is either occupied or unoccupied, and the persistence of the system lies in the balance of colonization by dispersal and local extinctions. Because the focal point of metapopulation theory is the dispersal capacity, the components of fragmentation that deal with patch size and edge configuration are largely ignored. The metapopulation system is thought of as a network of pointlike populations in space---they don't occupy any area and the key dynamics emerge as a product of their spatial configuration. However, the features of patch structure that metapopulation models tend to ignore can be captured by other means. For example, heterogeneity in patch sizes can correspond to different probabilities of local extinction. Other landscape dynamics can be captured using source-sink metapopulations (cite some source/sink, Gilpin). 

The field of landscape genetics shows progress toward unification of these two large bodies of theory through the use of network models.  In part due to the increasing affordability of high-throughput sequencing technology, the field of landscape genetics, introduced by (Manel et al. 2003), has sought to synthesize population genetic models with an understanding of landscape features using large-scale genomic data. The application of spatial networks has seen extensive application in this domain as well. Isolation-by-resistance (McRae 2006), useful in developing theory for real landscapes, habitat quality is not a 0/1. How do we think about resistance to gene flow? Resistance surfaces (Spear et al. 2010) are raster approach. Populations or individuals are modeled as points in space, each cell of the raster is assigned a resistance value, etc. etc.
Using a network is a convenient abstraction for the location of a population. We lose some details about the variance of the environment within the environment, but that is the reality of modeling. 



The task of modeling is to build a world. Science doesn’t discover, science creates.

Cartesian reductionism and dialectical approaches to ecological worldbuilding

