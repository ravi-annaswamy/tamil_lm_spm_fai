# tamil_lm_spm_fai
State of the Art Tokenizer, Language model and Classifier for Tamil language (spoken in India, and few other South Asian countries)


## Dataset
Download Wikipedia Articles Dump (>100,000 articles) and extract documents alone using WikiDataExtractor module. I have only use half of the articles for this model training.

## Tokenizer
Built tokenizer using Google sentence piece. Tried various vocabulary sizes and found that 8000 words
is optimal in early experiments. English Hindi etc work well with 30K word-parts, but since Tamil has 
even more complex morphology "(he) is about to go" is one word: "pogavirukkiraan".

## Language Model using Fastai AWD-LSTM (amazing code.)

* Perplexity of Language Model: ~37 

Thanks to Gaurav https://github.com/goru001 for clean packaged solution that we could build upon. Please feel free to use in whichever way to make code useful to anyone.

