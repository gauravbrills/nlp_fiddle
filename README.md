# nlp_fiddle
fiddle into nlp/nlu

## rasa fiddle 
experimenting with rasa api

### Installation
- Use anaconda and create 3.5 tensorflow env
- Install nlue `pip install rasa-nlu`
- Install sklearn 
```
pip install rasa_nlu[spacy]
python -m spacy download en_core_web_md
python -m spacy link en_core_web_md en
```
- Install tensorflow `pip install rasa_nlu[tensorflow]`

### Train the model
`python -m rasa_nlu.train -c nlu_config.yml --data nlu.md -o models --fixed_model_name nlu --project current --verbose`

### Create an interpreter
