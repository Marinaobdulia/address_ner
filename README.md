# Address-focused NER model


### Goal
Re-training an SpaCy NER model for identifying four categories inside an address:
- Street type (CALLE, AVENIDA, PASEO, PLAZA...)
- Street name (ALCALÁ, PRECIADOS, SOL...)
- Number
- Rest of address (PISO, PORTAL, ESCALERA...)

The training dataset was created using Madrid's street names and a combination of random techniques to obtain synthetic data.

### Code structure
Since the project was a POC, you can find the code divided across two notebooks:
- **Synthetic data creation**: [notebooks/training_set.ipynb](notebooks/training_set.ipynb)
- **Model re-training**: [notebooks/train_model.ipynb](notebooks/train_model.ipynb)

There is a final notebook containing all the code above: [notebooks/final.ipynb](notebooks/final.ipynb)

### Limitations
From performing some tests I found out several issues:
- The sample was not big enough to classify correctly to less common address structures.
- Since data is synthetic, the distribution of it might be far from the reality making the model prone to errors.


keywords: Calles de Madrid, callejero de Madrid, NER calles, NER direcciones, clasificar direcciones, direcciones español clasificar
