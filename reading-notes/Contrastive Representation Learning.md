Representation learning refers to the process of learning a **parametric mapping** from the raw input data domain to a feature vector or tensor, in the hope of capturing and extracting more abstract and useful concepts that can improve performance on a range of downstream tasks. Often the input domain has a high dimensional space (images, video, sound, text) and the encoded representations reside in a manifold of a much lower dimensionality. 

While all dimensionality reduction methods convert high-dimensional inputs to a lower-dimensional representation, some of these methods do not learn a mapping that meaningfully generalizes on new data samples, and that is what representation learning does.

The task of explicitly learning a good representation in comparison to implicitly learning a good representation to optimize performance for a task, can be tricky.

A good representation 
- has the properties of local smoothness of input and representation;
- is temporally and spatially coherent in a sequence of observations;
- has multiple, hierarchically-organised explanatory factors which are shared across tasks;
- has simple dependencies among factors and is sparsely activated for a specific input.

From these criteria the field of Representation Learning, especially in the Deep Learning circle, has itself developed a number of core principals used to learn a good representation and these are:
- **Distributed**: Representations that are expressive and can represent an exponential amount of configuration for their size. This is in contrast with other types of representations such as one-hot encoding, learned by many clustering algorithms;
- **Abstraction and Invariant**: Good representations can capture more abstract concepts that are invariant to small and local changes in input data; 
- **Disentangled representation**: While a good representation should capture as many factors and discard as little data as possible, each factor should be as disentangled as possible. Aside from promoting feature re-use in learning systems, it can also be beneficial for other purposes such as explainability.

A family of methods collectively called Contrastive Learning offers a simple method to encode these properties within a learned representation.