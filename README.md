# gram-error-tagger-models
Bidirectional LSTM Tagger models for Latvian Grammatical Error Detection

## Included
- Model 'ChatErrLabeling' marks errors in chat language text
- Model 'Preposition1' marks preposition errors in general text
- Model 'Agreement2' marks agreement errors in general text
- Model 'Verbform3' marks verb form errors in general text
- Model 'Nounform4' marks noun form errors in general text
- Model 'Adjending5' marks adjective ending errors in general text
- Model 'Rulescomma' marks missing comma errors in general text

## Prerequisites
Models are trained using toolkit 'sequence-labeler' https://github.com/marekrei/sequence-labeler. This toolkit is required to run the models.

## Data
Text for checking must be in two column CoNLL format. One word per line, separate column for token and label (can be 'O'), empty line between sentences. The tagger will add the label in the third column.
See files sampleinput.txt and sampleoutput.txt (results are obtained by model 'Rulescomma').

## Running tagger
python print_output.py labels <model_file> <input_file>

## Publications
Daiga Deksne. 2019. Bidirectional LSTM Tagger for Latvian Grammatical Error Detection. TSD 2019: International Conference on Text, Speech, and Dialogue, LNCS, volume 11697, 58-68.

## Acknowledgment
The research has been supported by the European Regional Development Fund within the project “Neural Network Modelling for Inflected Natural Languages” No. 1.1.1.1/16/A/215.
