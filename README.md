# BERT-Inferred_Minor_Status

Update: Paper currently under review for publication (2022-05-31)

Project Abstract: Automated solutions for data protections have been widely studied all while privacy is an increasing concern for the general public. Despite the increased attention paid toward data protection issues, little attention has been paid toward extending solutions to the vulnerabilities associated with minors and their personally identifiable information. The special vulnerability of children has been codified with legislation such as the GDPR in the European Union, yet research in data protection mechanisms like anonymization does not distinguish between children and adults. This paper seeks to respond to this need and proposes the use of a BERT named entity recognition model to make the subject distinction within unstructured text based on surrounding context. To demonstrate this proof-of-concept, we created a custom dataset, performed fine-tuning across a range of hyperparameters, and selected the best performing model. The resulting model achieved an 89\% f1 score in detecting minors and a 61\% f1 score in detecting adults. While the performance of this model may not be suited for a production environment, we have established a starting point for future research and the eventual integration of specific data protections for minors within an automated processing stack.

![project_graphic](https://github.com/JGillette71/BERT-Inferred_Minor_Status/blob/main/Data/bert_fine_tune_experiment.png)

Note: Results may vary. Recommended hyperparameters as follows. 
Max Input 256 (correlates to mean sequence length) 
Learn Rate 3.00e-05 (of range recommended in original BERT paper (Devlin et al.)
Epochs 3 (of range recommended in original BERT paper (Devlin et al.)
Batch Size 4
