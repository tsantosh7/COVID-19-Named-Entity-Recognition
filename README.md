# Named Entity Recognition for COVID-19 Bio Entities
The dataset was taken from https://github.com/davidcampos/covid19-corpus

# Dataset
The dataset was then split into several datasets each one representing one entity. Namely, Disorder, Species, Chemical or Drug, 
Gene and Protein, Enzyme, Anatomy, Biological Process, Molecular Function, Cellular Component, Pathway	and microRNA. Moreover, another dataset is also created with all those aforementioned that are non-overlapping in nature. 

# Dataset Formats
The datasets are available in two formats IOB and Spacy's JSONL format. 

IOB : https://github.com/tsantosh7/COVID-19-Named-Entity-Recognition/tree/master/Datasets/BIO
SpCy JSONL: https://github.com/tsantosh7/COVID-19-Named-Entity-Recognition/tree/master/Datasets/SpaCy

# Tutorials
1. Convert_to_JSON_IOB.ipynb : Coverts David Campos's BRAT annotations format to IOB and SpaCy's JSONL format
2. Train_NER_Model.ipynb : Trains SpaCy on the non-overlapping set for Named Entity Recognition (NER)

# Performance

### Chemicals or Drugs

|     precision-CHED:     	| 0.9012058695336336 	|
|     precision-CHED:     	| 0.9012058695336336 	|
|     recall-CHED:      	| 0.9284538242778028 	|
|     f1-measure-CHED:    	| 0.9146269537009233 	|


### Cellular Component  
|     precision-COMP:     	| 0.8954010095344924 	|
|     precision-COMP:     	| 0.8954010095344924 	|
|       recall-COMP:      	| 0.9488855869242199 	|
|     f1-measure-COMP:    	| 0.9213677679987958 	|

### Molecular Function 
|     precision-FUNC:     	| 0.8937691521961184 	|
|     precision-FUNC:     	| 0.8937691521961184 	|
|       recall-FUNC:      	| 0.9418729817007534 	|
|     f1-measure-FUNC:    	| 0.9171907756812917 	|

###         Anatomy
|     precision-ANAT:     	| 0.9170156071564523 	|
|     precision-ANAT:     	| 0.9170156071564523 	|
|       recall-ANAT:      	|  0.926657263751763 	|
|     f1-measure-ANAT:    	| 0.9218112244897461 	|

###      Pathway       
|     precision-PATH:     	| 0.8886986301369861 	|  	
|     precision-PATH:     	| 0.8886986301369861 	|
|       recall-PATH:      	| 0.9202127659574466 	|
|     f1-measure-PATH:    	| 0.9041811846689394 	|


###         Disorder        	
|     precision-DISO:     	| 0.9034559213380248 	|
|     precision-DISO:     	| 0.9034559213380248 	|
|       recall-DISO:      	| 0.9398786541643684 	|
|     f1-measure-DISO:    	| 0.9213074465470131 	|

###       Enzyme     
|     precision-ENZY:     	|  0.87378640776699  	|
|     precision-ENZY:     	|  0.87378640776699  	|
|       recall-ENZY:      	| 0.8823529411764702 	|
|     f1-measure-ENZY:    	| 0.8780487804877547 	|


###     Gene or Protein     
|     precision-PRGE:     	| 0.7596122247781795 	|
|     precision-PRGE:     	| 0.7596122247781795 	|
|       recall-PRGE:      	| 0.7721730415901119 	|
|     f1-measure-PRGE:    	|  0.765841133106883 	|

###    Biological Process  
|     precision-PROC:     	| 0.9172362555720653 	| 	
|     precision-PROC:     	| 0.9172362555720653 	|
|       recall-PROC:      	| 0.9362960715910814 	|
|     f1-measure-PROC:    	| 0.9266681678300183 	|

### Species    
|     precision-SPEC:     	| 0.9213247414955792 	|             	
|     precision-SPEC:     	| 0.9213247414955792 	|
|       recall-SPEC:      	|  0.951776453285858 	|
|     f1-measure-SPEC:    	| 0.9363030649152364 	|

###         Untyped     
|    precision-untyped:   	| 0.9073326280341524 	|    	
|    precision-untyped:   	| 0.9073326280341524 	|
|     recall-untyped:     	| 0.9355621792705037 	|
|   f1-measure-untyped:   	| 0.9212311928409375 	|

###  Combined Overall Result 	
|    precision-overall:   	| 0.8958739997913904 	|
|    precision-overall:   	| 0.8958739997913904 	|
|     recall-overall:     	| 0.9237470423747043 	|
|   f1-measure-overall:   	|  0.909597040779998 	|

# Contact
If you would like to know more or contribute, please send an e-mail or submit a pull request.