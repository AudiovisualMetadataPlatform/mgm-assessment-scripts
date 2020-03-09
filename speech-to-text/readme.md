# Speech-to-text

More information on evaluation and project recommendations on the [project wiki](https://wiki.dlib.indiana.edu/display/AMP/MGM+-+Speech-to-text)

MGM outputs, format conversion scripts, and comparison scripts (precision, recall, F1 scores + true positive, false positive, and false negative outputs) for three AMP project sample files:
- Astin Patten Lecture (IU Archives): Video documentation of an auditorium lecture at Indiana University
- Student-Admin Forum (IU Archives): Video documentation of a student and university administration forum
- Women and AIDS Teach-in (NYPL): Video documentation of an educational session on women's health issues  
  
The following speech-to-text services/tools were tested:
- [AWS Transcribe](https://aws.amazon.com/transcribe/)
- [CMU Sphinx](https://cmusphinx.github.io/)
- [Google Speech-to-Text](https://cloud.google.com/speech-to-text/)
- [Kaldi (WGBH/Pop-up Archive fork)](https://github.com/hipstas/kaldi-pop-up-archive)
- [Mozilla Deep Speech](https://github.com/mozilla/DeepSpeech)

This repository includes Python scripts for converting several of these outputs to a common plaintext format for word error rate (WER) scoring and comparison in the `stt_output_reshaping_scripts.ipynb` Jupyter notebook.   
  
The `calculate-wer.ipynb` Jupyter notebook includes Python scripts for comparing normalized outputs to a ground trutha and calculating WER.  

