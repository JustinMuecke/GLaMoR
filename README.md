# GLaMoR

This Repository contains all the code required to run the GLaMoR-Pipeline.
## Project Structure
```
├──GLaMoR-DataPipeline
│  ├──Data_Retrieval/ 
│  ├──Preprocessing/
│  ├──Initial_Publish/
│  ├──OAPT/
│  ├──OWL_Ontology_Modification/
│  ├──Prefix Removal/
│  ├──Translation/
│  ├──Tokenization/
│  ├──Embed/
│  ├──Analysis/
├──GLaMoR-Model_Training
│  ├──Data_Format_Translation/
│  ├──GLaMoR-HermiT/
│  ├──GLaMoR-ModernBert/
│  ├──GraphLanguageModels/
│  ├──Llama/
│  ├──Logistic_Regression/
│  ├──OWL2Vec-Star/
│  ├──Prodigy/
│  ├──WideMLP
├──.gitignore/
├──.gitmodules
├──README.md
├──LICENSE
```

## Requirements
The System is split into two components, the Data Pipeline and the Model Training. The requirements for the two components are listed below
### Data Pipeline
If you want to use the code as provided, it is enough to have docker-compose installed on the system and run 
```
> docker-compose build 
> docker-compose up -d 
```
in the root directory. Remember to update the mountings as well as environment variables according to your setup.

### Model Training
To train the models, a `requirements.txt` file is available for most of them. If it's missing, make sure you have the following installed:

- scikit-learn  
- pandas  
- numpy  
- torch

## Citation
A citation will be provided upon publication. In the meantime, please contact justin.muecke@uni-ulm.de for more information.
