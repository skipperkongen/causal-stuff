# causal-stuff

Trying different causal things

## Demos

- [BNLearn demo on sprinker data](./notebooks/bnlearn-demo.ipynb)

## Quiz

What is the binomial distribution?
- Do k trials, where in each trial you flip a coin n times, with probability p of heads, a count the number of heads. 

What is expit?
- Function that maps the reals into [0, 1], with expit(0) = 0.5

Prove that association is ATT + bias
```
association
= E[Y|T=1] - E[Y|T=0]
= E[Y1|T=1] - E[Y0|T=0] 
= E[Y1|T=1] - E[Y0|T=0] + E[Y0|T=1] - E[Y0|T=1]
= E[Y1 - Y0|T=1] + {E[Y0|T=1] - E[Y0|T=0]}
      ATT                  BIAS
``` 

What is confounding?
- Something that affects both X and Y.