# Summary

## Explainable AI

Why do we want explainability?
- To understand how a model works
- To understand the factors that are motivating the model's decisions
- To determine the trustworthiness of the model

### Stakeholders 

Various stakeholders benefit from explainable models, including:
- **Consumers**, who gain a better understanding of how they are impacted by the model.
- **Data Scientists/Model Developers**, who are able to more effectively debug and improve models based on their increased understanding.
- **Business Owners**, who are able to understand the models they are utilising, and evaluate their suitability for each application.
- **Risk Modellers**, who are able to evaluate the robustness of models more effectively when they have a deeper understanding of the decision-making process.
- **Regulators**, who can more easily evaluate the impact of models on consumers, and verify the reliability of models.
- etc.

### Properties of XAI Approaches

Explainability methods can be categorised according to when the explanation is generated relative to the model output ({ref}`content:week11:summary:intrinsic-vs-post-hoc`). 

They can be further categorised based on whether they provide explanations at the level of individual instances, or look at the model and its parameters as a whole ({ref}`local-vs-global`).

Finally, some explanation techniques are specific to the inner workings of a given model (**Model Specific Explanations**) and others rely only on inputs and outputs, therefore making them applicable to any model with that interface (**Model Agnostic Explanations**).

(intrinsic-vs-post-hoc)=
#### Intrinsic vs. Post-hoc

Intrinsic Interpretability 
: is achieved when a model is constructed in a way that is inherently understandable. This includes models such as decision trees and linear models, where the logic performed by the algorithm can easily be traced by a human.

Post-hoc Interpretability
: requires the construction of a second model to provide explanations for a model that is inherently uninterpretable. This approach is often applied to deep learning models so that explanations can be achieved without sacrificing performance.

(local-vs-global)=
#### Local vs. Global

Local Explanations 
: examine the result for individual instances, and help to understand the causal relationship between the input to the model and the corresponding prediction.

Global Explanations 
: inspect the structures and parameters present in the model, facilitating an understanding of its inner mechanisms.