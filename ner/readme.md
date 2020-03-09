## Named entity recognition (NER)

More information on evaluation and project recommendations on the [project wiki](https://wiki.dlib.indiana.edu/display/AMP/MGM+-+Entity+Extraction)

Source transcripts, MGM outputs, format conversion scripts, and comparison scripts (precision, recall, F1 scores + true positive, false positive, and false negative outputs) for transcripts (ground truth, AWS Transcribe, Kaldi) from three AMP project sample files:
- Astin Patten Lecture (IU Archives): Video documentation of an auditorium lecture at Indiana University
- Student-Admin Forum (IU Archives): Video documentation of a student and university administration forum
- Women and AIDS Teach-in (NYPL): Video documentation of an educational session on women's health issues  
  
The following NER services/tools were tested:
- [AWS Comprehend](https://aws.amazon.com/comprehend/)
- [Google Natural Language API](https://cloud.google.com/natural-language/)
- [IBM Watson Natural Language Understanding](https://cloud.ibm.com/catalog/services/natural-language-understanding)
- [SpaCy](https://spacy.io)
- [Stanford CoreNLP](https://nlp.stanford.edu/software/index.shtml)  
  
This repository includes Python scripts for converting several of these outputs to a common CSV format for precision/recall/F1 scoring and comparison in the `reshape-ner-output.ipynb` Jupyter notebook.  
  
The `ner-metrics.ipynb` Jupyter notebook includes Python scripts for comparing normalized outputs to a ground truth.  
  
The `spacy` directory contains Python scripts for both running SpaCy NER with the default model as well as alongside SpaCy's EntityRuler (rule-based entity matching) with custom vocabularies.  