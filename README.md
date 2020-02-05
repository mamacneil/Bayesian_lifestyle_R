# Your Bayesian Lifestyle
## Getting started with Bayesian statistical models in R or Python

Material for this tutorial have been cribbed from Chris Fonnesbeck and Colin Carroll, the original contents of which can be found (here)[https://github.com/fonnesbeck/Bayes_Computing_Course.git]


## Material for course on Bayesian Computation

For the R/Stan version, you can [download a zip file](https://github.com/mamacneil/Bayesian_lifestyle_R/archive/master.zip) of its contents, and unzip it on your computer.

## Setup

First, you should have both R (https://cloud.r-project.org/bin/) and RStudio (https://www.rstudio.com/products/rstudio/download/preview/) installed.

For R/Stan users we'll follow Richard McElreath's [`rethinking` setup on github](https://github.com/rmcelreath/rethinking):

You can find a manual with expanded installation and usage instructions here: http://xcelab.net/rm/software/

Here's the brief verison.

You'll need to install rstan first. Go to https://mc-stan.org/users/interfaces/rstan.html and follow the instructions for your platform. The biggest challenge is getting a C++ compiler configured to work with your installation of R. The instructions at https://github.com/stan-dev/rstan/wiki/RStan-Getting-Started are quite thorough. Obey them, and you'll likely succeed.

Then you can install rethinking from within R using:

install.packages(c("coda","mvtnorm","devtools","loo","dagitty"))
library(devtools)
devtools::install_github("rmcelreath/rethinking",ref="Experimental")

If there are any problems, they likely arise when trying to install rstan, so the rethinking package has little to do with it. See the manual linked above for some hints about getting rstan installed. But always consult the RStan section of the website at mc-stan.org for the latest information on RStan.



## Course Outline

This is subject to change. I will seek input and try to accommodate digression where there is interest. Roughly, the first half of the course jumps right in with applied examples, then steps back to cover some of the theory behind Bayesian methods before going carefully through another applied case study. 

### Wednesday, February 8
1. **Basic Bayes** 9:00am - 12:00pm
	- Bayes formula
	- Likelihoods, Priors, and Posteriors
	- Radon, it's everywhere
	- IQ drugs, they're real
	- Phase-shifts, with fish

2. **Hierarchcial Models**  1:00pm - 4:00pm
    - Motivation and case studies
    - Partial pooling
    - Building hierarchical models
    - Parameterizations
    - Model checking

 
### Thursday, January 9

3. **The Bayesian Workflow**  9:00am - 12:00pm
    - Prior predictive checks
    - Iterating models
    - Posterior predictive checks
    - Using the model

4. **Your data** 1:00pm - 4:00pm
    - Questions relating to your own data
    - How to get started with your unique problem
    - Resources

