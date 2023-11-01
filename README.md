## E2E Machine Learning Project
## End to End MAchine Learning Project

## day 1 git and setup
1. set up the github repo {}
    a. new environment


        create a new git repo;
        create a local folder with the same repo name
        open vscode and open the repo path
        open a terminal in vscode -> conda create -p venv python==3.8 -y -> {repo}/venv folder created in the repo
        -> conda activate venv
        
        echo "# airbnb_ds" >> README.md
        git init
        git add README.md
        git commit -m "first commit"
        git branch -M main
        git remote add origin https://...
        git remote -v
        git push -u origin main

        create .gitignore file in github.com UI, choose python and commit this change in remote 
        git pull 
    
    
    b. setup.py (will build my application as a package)
        create {repo}/setup.py
        from setuptools import find_packages,setup
        
        create {repo}/src folder -> create a __init__.py file inside src folder, then src can be imported as a module. The main dev work will be inside src; -> when build is done, a {repo}.egg-info is created. 
        
        create {repo}/requirements.txt -> append '-e .' as the last line, this will trigger setup.py and build
        pip install -r requirements.txt

## day2 project structure, logging and exception handling
    create {repo}/src/components folder -> create a __init__.py file inside this folder
        data_ingestion.py
        data_transformation.py
        model_trainer.py
        model_pusher.py
    create {repo}/src/pipeline folder -> create a __init__.py file inside this folder
        train_pipeline.py
        predict_pipeline.py
    create
        exception.py
        logger.py -> will create and save logs in {repo}/log folder
        utils.py

## day3 Problem Statement and EDA
    create {repo}/notebooks folder -> create EDA.ipynb and ModelTraining.ipynb 
    create {repo}/notebooks/data folder -> local copy of source data
    
## day4 data ingestion
    
## day5 data transformation

## day6 model trainer

## day7 model hypertuning
   
## day8 model pusher
   AWS beanstalk, codepipeline


    
    