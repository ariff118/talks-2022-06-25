---
date: "2022-06-25"
draft: false
excerpt: Grid is the very first CSS module created specifically to solve the layout
  problems we’ve all been hacking our way around for as long as we’ve been making
  websites.
subtitle: Two Continuous Moderators
title: Model 2
weight: 3
---

## Model 2  

### Introduction  

**Moderators $W$ and $Z$**  

- Example Variables: 1 predictor *X*, 2 Moderators *W* & *Z*, 1 outcome *Y*  

- The primary IV (variable *X*) is continuous  

- The moderators are continuous  

::: callout-example  
IV: Commitment  
MoDV1: Role Ambiguity  
MoDV2: Role Conflict  
DV: OP
:::  

### How to run in SPSS Process Macro?  

1. Insert model framework image here.  

2. Analyze > Regression > PROCESS v4.0 by Andrew fF. Hayes  
    Insert image here...  

3. Insert variables (*Y*, *X*, *W*, and *Z*) and choose `Model 2`  
    Insert image here...  

4. Click Options button:  
    - check on `Generate code for visualizing interactions`  
    - Mean center - choose `Only continuous variables that define product`.  
    - Conditioning values - choose `-1SD, Mean, +1SD`  
    - click `Continue`
    insert image here ...  

5. click `OK` to run analysis  

### Reading the output  

- Model Summary, provides summary of model with *R*, $R^2$, $F$ statistic, and $p$ value for the overall model. Next, is the coefficients, with impact of Commitment, Role Ambiguity, Role Conflict, and the interaction effects to assess if there is moderation or not.  

- Culture has a significant impact on *OP*.  

- *RA* and its interaction with Culture (int_1) has a significant impact on *OP*. This shows that *RA* moderates the relationship between Culture and *OP*.  

- *RC* and its interaction with Culture (int_2) had an insignificant impact on *OP*. This shows that *RC* doesn't moderate the relationship between Culture and *OP*.  

Insert Second Output Image Here...  

- Test of unconditional interaction, this shows the change in $R^2$ due to interaction (X*W), this is significant.  

- Test of unconditional interaction, this shows the change in $R^2$ due to interaction (X*Z), this is significant.  

- Next, the conditional effects of the focal predictor at values of the moderator.