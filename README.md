# Named Entity Recognition for COVID-19 Bio Entities

The dataset was taken from <https://github.com/davidcampos/covid19-corpus>

## Dataset

The dataset was then split into several datasets each one representing one entity. Namely, Disorder, Species, Chemical or Drug, 
Gene and Protein, Enzyme, Anatomy, Biological Process, Molecular Function, Cellular Component, Pathway	and microRNA. Moreover, another dataset is also created with all those aforementioned that are non-overlapping in nature. 


## Dataset Formats
The datasets are available in two formats IOB and Spacy's JSONL format. 

IOB : <https://github.com/tsantosh7/COVID-19-Named-Entity-Recognition/tree/master/Datasets/BIO>

SpCy JSONL: <https://github.com/tsantosh7/COVID-19-Named-Entity-Recognition/tree/master/Datasets/SpaCy>

## Tutorials
1. Convert_to_JSON_IOB.ipynb : Coverts David Campos's BRAT annotations format to IOB and SpaCy's JSONL format

2. Train_NER_Model.ipynb : Trains SpaCy on the non-overlapping set for Named Entity Recognition (NER)

## Performance

| Chemicals or Drugs          	|      	|
|-----------------------------	|------	|
| precision-CHED:             	| 0.90 	|
| recall-CHED:                	| 0.93 	|
| f1-measure-CHED:            	| 0.91 	|
| **Cellular Component**      	|      	|
| precision-COMP:             	| 0.90 	|
| recall-COMP:                	| 0.95 	|
| f1-measure-COMP:            	| 0.92 	|
| **Molecular Function**      	|      	|
| precision-FUNC:             	| 0.89 	|
| recall-FUNC:                	| 0.94 	|
| f1-measure-FUNC:            	| 0.92 	|
| **Anatomy**                 	|      	|
| precision-ANAT:             	| 0.92 	|
| recall-ANAT:                	| 0.93 	|
| f1-measure-ANAT:            	| 0.92 	|
| **Pathway**                 	|      	|
| precision-PATH:             	| 0.89 	|
| recall-PATH:                	| 0.92 	|
| f1-measure-PATH:            	| 0.90 	|
| **Disorder**                	|      	|
| precision-DISO:             	| 0.90 	|
| recall-DISO:                	| 0.94 	|
| f1-measure-DISO:            	| 0.92 	|
| **Enzyme**                  	|      	|
| precision-ENZY:             	| 0.87 	|
| recall-ENZY:                	| 0.88 	|
| f1-measure-ENZY:            	| 0.88 	|
| **Gene or Protein**         	|      	|
| precision-PRGE:             	| 0.76 	|
| recall-PRGE:                	| 0.77 	|
| f1-measure-PRGE:            	| 0.77 	|
| **Biological Process**      	|      	|
| precision-PROC:             	| 0.92 	|
| recall-PROC:                	| 0.94 	|
| f1-measure-PROC:            	| 0.93 	|
| **Species**                 	|      	|
| precision-SPEC:             	| 0.92 	|
| recall-SPEC:                	| 0.95 	|
| f1-measure-SPEC:            	| 0.94 	|
| **O-tag**                   	|      	|
| precision-untyped:          	| 0.91 	|
| recall-untyped:             	| 0.94 	|
| f1-measure-untyped:         	| 0.92 	|
| **Combined Overall Result** 	|      	|
| precision-overall:          	| 0.90 	|
| recall-overall:             	| 0.92 	|
| f1-measure-overall:         	| 0.91 	|

## Using the model

#### download SpaCy model: 
<https://drive.google.com/open?id=1QoIeOAUZqaFLGrS-gJH1aAlE1_bn22ZI>


#### install the model:
``` bash
pip install en_covido-0.0.0.tar.gz 
```

#### load the model:

```bash
import spacy
import en_covido
```

#### perform NER

```bash
nlp = en_covido.load()

doc = nlp("The coronavirus SPEC pandemic has become a growing public health concern worldwide, and there are insufficient epidemiological data on critical illness DISO . We sought to investigate the clinical course and features of critical patients with Corona Virus Disease 2019 DISO (COVID-19).")

for ent in doc2.ents:
    print(ent.label_, ent.text)
```
#### check results

```
SPEC coronavirus
DISO critical illness
DISO Corona Virus Disease 2019
DISO COVID-19
```



## Contributing
Pull requests are welcome. 

Please make sure to update tests as appropriate.

# Contact
If you would like to know more or contribute, please send an e-mail or submit a pull request.

## License
[MIT](https://choosealicense.com/licenses/mit/)