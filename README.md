# who-is-leo
A finetuned LLM trained on information about Leonardo Moreno and who he is. 
- Base Model: https://huggingface.co/TinyLlama/TinyLlama-1.1B-Chat-v1.0 
- Dataset used: https://huggingface.co/datasets/j2moreno/leo-training-data
- Finetuned Model: https://huggingface.co/j2moreno/TinyLlama-1.1B-Chat-v1.0-leo-finetuned 
- Space where you can test model on hugging face: https://huggingface.co/spaces/j2moreno/who-is-leo 

**NOTE:** This is an ongoing project and will be updating to include more test data and be more accurate on its repsonses

## Data processing 
Data was created by me and formatted in the same way that the TinyLlama model was trained. 

Data can be found at: https://huggingface.co/datasets/j2moreno/leo-training-data

## Model Training 
The model was trained on the test dataset and ran on AWS SageMaker. The model, once trained, was exported to hugging face repo and currently lives there. 

More info on training can be found in the `training.ipynb`. 

To run the training an instance of Smazon's ml.m5d.2xlarge was used with 8 vCPUs and 32GB of RAM with 60GB of storage. 

Model location: https://huggingface.co/j2moreno/TinyLlama-1.1B-Chat-v1.0-leo-finetuned 

## Space 
Using gradio libraries, I was able to create and host an app representation of the finetuned model for testing. Please go to hugging face spaces found here to try the model out: https://huggingface.co/spaces/j2moreno/who-is-leo 




