# streamlit-sample-qa-bert-frontend
sample frontend demo for bert qa using streamlit

## credit 
### copied from https://pub.towardsai.net/build-and-deploy-a-bert-question-answering-app-using-streamlit-1aba1d76b84 
### this is for record and study only. To cite, refer to original post


## install
Ubuntu 20.04

In this project, I will show how with Streamlit and the HuggingFace Transformers model, we can deploy an interactive web app to Render for free to a state-of-the-art neural question answering system to a question from a particular text/document/corpus.

Let’s get started!


### install git lfs and pull it right after git clone
- download from https://git-lfs.com/
- unzip compressed file
- sudo ./install.sh
- sudo git lfs pull

### docker build
sudo docker build -t bertqa:app .

### docker image list
sudo docker image ls

### docker image push to hub
sudo docker tag bertqa:app weili1988/bertqa:app

### docker image pull/run from hub
sudo docker container run -p 8501:8501 -d weili1988/bertqa:app

### go to web browser with address: http://localhost:8501/
