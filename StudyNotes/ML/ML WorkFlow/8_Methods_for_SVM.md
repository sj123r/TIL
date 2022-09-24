# Comparison between OvR and OvO for SVM application [paper review/논문리뷰]
## 논문리뷰(determining hand gestures) 

The [paper study](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7235125/) does a meta analysis of scientific literatures that have compared the accuracy of SVM with varying kernels(linear, polynomial, RBF) and classification strategies(OvO, OvR).

## Conclusion:
It is generally accepted that OvO is a more suitable for SVM compared to OvR because of the idea that "kernel methods don’t scale in proportion to the size of the training dataset". 

While it was proven true that, to some extent, OvO was superior in the classifications; it wasn't necessarily true for all cases.

In fact, OvR method with a parallel topology applied, where kernels are adjusted accordingly to the datset, showed the highest accuracy in multi-classification. 

This refutes the common notion that OvR is used in small datasets that doesn't require high accuracy whereas OvO is used in datasets that need high accuracy rates.

This implies that OvR might be the best suitable choice in all cases, if parallel topology can be applied.