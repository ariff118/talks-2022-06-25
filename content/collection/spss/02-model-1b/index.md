---
date: "2022-06025"
excerpt: In this block, we'll use the postcards package to make a single 'about' home
  page with only R Markdown.
subtitle: One Moderator (Categorical)
title: Model 1b
weight: 2
---

## Model 1b: 1 Moderator with Categorical Moderator  

### Introduction  

- Example Variables: 1 predictor *X*, 1 moderator *W*, 1 outcome *Y*  

- *Preliminary Notes*  
  - Model 1b assumes that:  
    - The primary IV (variablle *X*) is continuous  
    - The moderator is categorical with multiple categories  

::: callout-Example  
IV: Commitment  
MoDV: Bank (Size - Small, Medium, Large)  
DV: OP
:::  

::: callout-Objective  
The impact of Commitment on Organizational Performance is moderated by the size of the Bank
:::  

### How to run in SPSS Process Macro?  

1. Insert model framework image here.  

2. Analyze > Regression > PROCESS v4.0 by Andrew fF. Hayes  
    Insert image here...  

3. Insert variables (*Y*, *X*, and *W*) and choose `Model 1`  
    Insert image here...  

4. Click Options button:  
    - check on `Generate code for visualizing interactions`  
    - Mean center - choose `Only continuous variables that define product`.  
    - click `Continue`

5. Click `Multicategorical` button:  
    - Under Variable W  
        - check box  
        - Coding system: `Indicator` (this will create a dummy coding for the moderator variable)
    - click `Continue`
    insert image here ...  

5. click `OK` to run analysis  

### Reading the output  

**Insert First Output Image Here**  

- Description of Model along with the different variables where *Y* is Dependent Variable, *X* is Independent Variable, and *W* is the Moderating Variable.  

- Bank is Categorical with Small, Medium, and Large Sized Banks.  

- Coding of categorical *W* variable for analysis:  

:::{.callout-note collapse="true"}
## Expand To Learn About Dummy Coding

    | Bank   | W1  | W2  |  
    |:------:|:---:|:---:|  
    | 1.000  | .000| .000|  
    | 2.000  |1.000| .000|  
    | 3.000  | .000|1.000|  
    
  W1 - Medium vs Small (Small is the Reference Category)  
  W2 - Large vs Small  
  
:::

**Insert Second Image Output Here**  

- Model Summary, provides summary of the model with $R$, $R^2$, $F$ statistic, and $p$ value for the overall model. Next, is the coefficients, with impact of *Commitment*, *Bank Size*, and the interaction effects to assess if there is moderation or not.  

- Differences in *OP* between Medium and Small banks is insignificant (W1, *p* > 0.05). Medium sized banks have a higher *OP* in comparison to small sized banks.  

- Differences in *OP* between Large and Small banks is significant (W2, $p$ < 0.05). Large sized banks has a lower *OP* in comparison to small sized banks.  

::: callout-note  
Can verify that the effect whether higher or lower in *OP* through the mean comparison. This can be done easily using SPSS:  
Go to Analyze > Compare Means > Means  
Dependent: *OP*  
Independent: *Bank*  
Click `OK`  
:::  

- In this example, one interaction effect (Int_1) is significant. Impact of Commitment on Performance in Medium Sized Banks is considerably different (lower) from Small Sized Banks.  

- However, impact of Commitment on Performance in Large Sized Banks is not significantly different from Small Sized Banks.  

- Test of unconditional interaction. This shows the change in $R^2$ due to interaction _(x*w)_, this is also significant.  

- Next, the conditional effects show that for Small and Large Sized Banks, the effects of Commitment on Organzational Performance is significant.  

#### Data Visualization  

There are two ways to draw the interaction path in order to give you a clearer visulization on the effects of moderator on the relationship between the predictor and the outcome variable.  

1. Using the SPSS syntax  
    - copy the script from the process macro output.  
    - in SPSS, open a new syntax file  
    - paste the script into your syntax file  
    - click `Run` button to create your interaction graph  
    ...insert image here.  

2. Using the StatsTool package created by James Gaskin  
    - link to download the STatTools Package ->  

::: callout-interpretation  
1. The study assessed the moderating role of Bank Size on the relationship between Commitment and Organizational Performance (OP). Test of unconditional interaction shows the change in $R^2$ due to interaction (x*w) is significant. The result revealed that although Medium Sized Banks have a higher OP in comparison to Small Size Banks. Differences in OP between Medium and Small bank were insignificant (W1, $p$ > 0.05)   

2. Furthermore, large sized banks have a lower *OP* in comparison to small size banks. Differences in *OP* between Large and Small banks were significant (W2, *p* < 0.05). In this example, one interaction effect (Int_1) is significant, such that, impact of Commitment on Performance in Medium sized banks is considerably different (lower) from Small sized banks. However, impact of Commitment on Performance in Large sized banks is not significantly different from Small sized banks.  
:::  