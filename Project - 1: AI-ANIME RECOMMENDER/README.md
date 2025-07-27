# AI ANIME RECOMMENDER Using Grafana Cloud, MiniKube, ChromaDB and LangChain


<img width="779" height="179" alt="image" src="https://github.com/user-attachments/assets/3c0ee450-66ae-4fb2-8b16-73098f8a2839" />

## Project and API Setup (Grog and HuggingFace)

Install the vc_redist package

```
https://aka.ms/vs/17/release/vc_redist.x64.exe
```

Install Python on your Local machine


<img width="308" height="62" alt="image" src="https://github.com/user-attachments/assets/2e727a59-6575-4d1a-b235-9fde58d75fde" />


To Create a folder named ANIMERECOMMENDER and inside the folder to create venv

```
>python -m venv venv
>Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
>venv\Scripts\activate
```


<img width="737" height="355" alt="image" src="https://github.com/user-attachments/assets/dd558b3a-b816-4e7c-9fe0-5db0476f512d" />

To Create .env file in the root directory

To create a Groq API key

https://console.groq.com/keys

To create a Huggingface API token

https://huggingface.co/settings/tokens

.env file

```

```

To create a folder named data in the root directory

To create a file named anime_with_synopsis.csv inside the data folder or place the csv file using below link

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/data/anime_with_synopsis.csv
```

To create a file named requirements.txt in the root directory

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/requirements.txt
```

To create a file called setup.py in the root directory to install all your dependencies

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/setup.py
```

To trigger the setup.py

Inside the root directort and run the below command which will install the build dependencies

```
pip install -e .
```

To create a folder named "src" in the root directory and create a file called "_init_.py" inside the src folder

To create a folder named "utils" in the root directory and create a file called "_init_.py" inside the utils folder

To create a file named "custom_exception.py" inside the utils folder

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/utils/custom_exception.py
```

To create a file named "logger.py" inside the utils folder

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/utils/logger.py
```

To create a folder named "config" in the root directory and create a file called "_init_.py" inside the src folder

To create a folder named "app" in the root directory and create a file called "_init_.py" inside the utils folder

To create a folder named "pipeline" in the root directory and create a file called "_init_.py" inside the utils folder

To install the build dependencies again

```
>pip install -e .
```

Now your root directort should like this


<img width="748" height="373" alt="image" src="https://github.com/user-attachments/assets/fb6f5353-0028-4b85-8d33-82d97ee900da" />


To create a file called "config.py" inside the config folder

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/config/config.py
```

To create a file called "data_loader.py" inside the src folder

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/src/data_loader.py
```

To create a file called "vector_store.py" inside the src folder

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/src/vector_store.py
```

To create a file called "prompt_template.py" inside the src folder

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/src/prompt_template.py
```

To create a file called "recommender.py" inside the src folder

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/src/recommender.py
```

To create a "pipeline.py" inside the pipeline folder

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/pipeline/pipeline.py
```

To create a file called "build_pipeline.py" inside the pipeline folder

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/pipeline/build_pipeline.py
```

To build the build_pipeline

To run the below command in the root directory terminal

```
python pipeline/build_pipeline.py
```

The pipeline built successfully!


<img width="676" height="389" alt="image" src="https://github.com/user-attachments/assets/44c5ae35-45b7-47f5-bc3f-33e9cc50e9e9" />


To create a file called "app.py" inside the app folder

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/app/app.py
```

To run the app.py from the root directory

```
>streamlit run app/app.py
```

To open your browser and hit http://localhost:8501/


<img width="701" height="376" alt="image" src="https://github.com/user-attachments/assets/ff6a907f-7efe-4eb4-9211-62ceb9664b46" />


Just add the anime preferences "light hearted anime with school settings" and then you will get recommendations


To create a Dockerfile in the root directory

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/Dockerfile
```

To create a k8's deployment and service file

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/llmops-k8s.yaml
```

To create .gitignore file in the root directory to add the content that you dont want to push to github

```
https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS/blob/main/.gitignore
```

To push the code to the GitHub repo

To create a repo named "ANIME-RECOMMENDER-SYSTEM-LLMOPS" in GitHub

```
>git init
>git commit -am "Files are uploaed"
>git branch -M main
>git remote add origin <URL>
>git push -u origin main
```
