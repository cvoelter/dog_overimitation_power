# Power simulations for the project: Overimitation in dogs: Ontogentic and phylogenetic influences

| Study | Topic        | Prediction                                   | Response variable                  | error structure | test condition          | test condition 2 | control condition   | N        | power | design  | n. trials | model                                                                         |
| ----- | ------------ | -------------------------------------------- | ---------------------------------- | --------------- | ----------------------- | ---------------- | ------------------- | -------- | ----- | ------- | --------- | ----------------------------------------------------------------------------- |
| 1     | relationship | assistance dogs > family dogs > shelter dogs | irrelevant action copying (binary) | binomial        | assistant: 0.8          | shelter: 0.3     | family:  0.58       | 20/20/20 | 99    | between | 4         | glmer(resp ~ group + sex +z.age+z.trial+(1+z.trial|subject), family=binomial) |
| 2     | oxytocin     | oxytocin > placebo                           | irrelevant action copying (binary) | binomial        | oxytocin: 0.75          |                  | placebo: 0.58       | 38/38    | 81    | between | 4         | glmer(resp ~ group + sex +z.age+z.trial+(1+z.trial|subject), family=binomial) |
| 3     | causality    | irrelevant action experience = no experience | irrelevant action copying (binary) | binomial        | experienced: 0.4        |                  | no experience: 0.58 | 38/38    | 80    | between | 4         | glmer(resp ~ group + sex +z.age+z.trial+(1+z.trial|subject), family=binomial) |
| 4     | obedience    | less obedient = more obedient                | irrelevant action copying (binary) | binomial        | obedience trained: 0.75 |                  | family dogs: 0.58   | 38/38    | 81    | between | 4         | glmer(resp ~ group + sex +z.age+z.trial+(1+z.trial|subject), family=binomial) |
| 5     | wolf         | dog>wolf                                     | irrelevant action copying (binary) | binomial        | wolves: 0.2             |                  | pack dogs: 0.5      | 13/13    | 84    | between | 4         | glmer(resp ~ group + sex +z.age+z.trial+(1+z.trial|subject), family=binomial) |
| 6     | puppy        | adult>puppy                                  | irrelevant action copying (binary) | binomial        | puppy: 0.3              |                  | adult dogs: 0.58    | 40/40    | 99    | between | 4         | glmer(resp ~ group + sex +z.age+z.trial+(1+z.trial|subject), family=binomial) |

## Structure

```         
.
├── Study 1           <-- Power analysis for Study 1 (binomial GLMM w/ irrelevant action copying as DV).
├── Study 2           <-- Power analysis for Study 2 and 4 (binomial GLMM w/ irrelevant action copying as DV).
├── Study 3           <-- Power analysis for Study 3 (binomial GLMM w/ irrelevant action copying as DV).
├── Study 5           <-- Power analysis for Study 5 (binomial GLMM w/ irrelevant action copying as DV).
├── Study 6           <-- Power analysis for Study 6 (binomial GLMM w/ irrelevant action copying as DV).
```
