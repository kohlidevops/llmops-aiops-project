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
GROQ_API_KEY="aaaaaaaaaaaaaaaaaaaaaaabbbbbbbbbbbbbbbbbb"
HUGGINGFACEHUB_API_TOKEN="aaaaaaaaaaaaaaaaaaabbbbbbbbbbbbbbb"
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

**To push the code to the GitHub repo**

To create a repo named "ANIME-RECOMMENDER-SYSTEM-LLMOPS" in GitHub

```
>git init
>git commit -am "Files are uploaed"
>git branch -M main
>git remote add origin <URL>
>git push -u origin main
```

<img width="856" height="446" alt="image" src="https://github.com/user-attachments/assets/12e7077e-c387-4d0e-b4a0-c16841ef087e" />


## To create a VM in GCP

```
VM > Create a new VM
Name > llmops-anime-recommender
Region and zone > choose your own
Instance type > E2
Machine type > e2-standard-4 (4vcpu, 2 core and 16 RAM)
OS > Ubuntu and its version > Ubuntu-24.04 LTS Minimal - x86/64, amd64 noble minimal image built on 2025-07-25
Boot disk type > Balanced Persistent Disk
Size > 150 GB
Networking > Allow HTTP, HTTPS and Loadbalancer Healthcheck
IP forwarding > Enable
Rest of things > Default and Create a VM
```

**To SSH to machine and install docker**

```
https://docs.docker.com/engine/install/ubuntu/
```

**SSH and install**

```
# Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update

sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
sudo docker run hello-world
sudo groupadd docker
sudo usermod -aG docker $USER
newgrp docker
docker run hello-world
sudo systemctl enable docker.service
sudo systemctl enable containerd.service
```


<img width="635" height="263" alt="image" src="https://github.com/user-attachments/assets/435ca01e-75f5-47c2-8c18-51ea3d6edcee" />


## To install MiniKube on the GCP VM

```
https://minikube.sigs.k8s.io/docs/start/?arch=%2Flinux%2Fx86-64%2Fstable%2Fbinary+download
```

**SSH and install minikube**

```
OS > Linux
Architecture > X86
Release > Stable
Installer type > Binary

curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube && rm minikube-linux-amd64
minikube start
```


<img width="775" height="233" alt="image" src="https://github.com/user-attachments/assets/d64ae82c-e415-4f89-a364-16d3f5d80f75" />


**To install kubectl**

```
https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/
```

**SSH and install kubectl**

```
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl.sha256"
sudo snap install kubectl --classic
kubectl version --client
```


<img width="803" height="153" alt="image" src="https://github.com/user-attachments/assets/f0c8052a-fb44-4e57-8ab2-f30bc1f3ca28" />


## To GitHub integration with VM

```
git clone https://github.com/kohlidevops/ANIME-RECOMMENDER-SYSTEM-LLMOPS.git
cd ANIME-RECOMMENDER-SYSTEM-LLMOPS
git config --global user.email "latchudevops1@gmail.com"
git config --global user.name "kohlidevops"
git add .
git commit -am "updated"
git push origin main
<you have to create classic token and proceed>
```


<img width="771" height="364" alt="image" src="https://github.com/user-attachments/assets/e0fdc006-8d18-4422-8b6b-9dd8d0b772e5" />


## To create a Firewall rule in GCP

```
Firewall > Create a new Firewall Rule
Name > llmops-firewall
Network > default
Priority > 1000
Direction of traffic > Ingress
Action on match > Allow
Targets > All instances in the network
Source filter > IPv4
Source IPv4 ranges > 0.0.0.0/0
Protocol and Ports > Allow all
Then create
```


<img width="609" height="377" alt="image" src="https://github.com/user-attachments/assets/328430a5-8f81-4159-acfe-373a7c673403" />


**To Build and Deploy your App on VM**

```
cd ANIME-RECOMMENDER-SYSTEM-LLMOPS
eval $(minikube docker-env)
docker build -t llmops-app:latest .
docker images
kubectl create secret generic llmops-secrets \
  --from-literal=GROQ_API_KEY="xxxxxxxxxx" \
  --from-literal=HUGGINGFACEHUB_API_TOKEN="xxxxxxxxx"
kubectl apply -f llmops-k8s.yaml
kubectl get pods
```


<img width="732" height="106" alt="image" src="https://github.com/user-attachments/assets/8d24ea33-06d1-427b-999e-9a8d421cb147" />


```
# Do minikube tunnel on one terminal
minikube tunnel
# Open another terminal
kubectl port-forward svc/llmops-service 8501:80 --address 0.0.0.0
## Now copy external ip and :8501 and see ur app there....
```


<img width="746" height="146" alt="image" src="https://github.com/user-attachments/assets/7f46f2e3-f8cc-4379-9f97-63d56c5bd6d0" />


<img width="921" height="187" alt="image" src="https://github.com/user-attachments/assets/b602588e-6897-4ec8-9f28-7c3f2ac38616" />


<img width="778" height="432" alt="image" src="https://github.com/user-attachments/assets/28cf628d-4f21-490e-ac16-1dd9696a2d47" />


## Monitoring Kubernetes using Grafana Cloud

**Create namespace and install Helm on VM with the help of new terminal as already being used other terminals**

```
kubectl create ns monitoring
kubectl get ns
```


<img width="638" height="138" alt="image" src="https://github.com/user-attachments/assets/2e23b50d-0e16-47fc-ae2b-70b79f0206cd" />


**Install Helm**

```
https://helm.sh/docs/intro/install/
```

**SSH and install Helm**

```
curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
chmod 700 get_helm.sh
./get_helm.sh
```


<img width="881" height="163" alt="image" src="https://github.com/user-attachments/assets/aeac54da-f85d-441b-b882-4dfcf3885be6" />


## To create a Grafana Cloud account with GitHub or anything

```
Come to grafana cloud --> Left pane observability --> Kubernetes--> start sending data
In backend installation --> Hit install
Give your clustername and namespace there : minikube and monitoring in our case
Select kubernetes
Keep other things on as default
Here only create new access token give name lets give minikube-token & Create it and save it somewhere..
Select helm and deploy helm charts is already generated...
```

**SSH to VM**

```
vi values.yaml

You can copy this code from Grafana Cloud > Deployment to copy section
Paste all from there to your file now remove last EOF part & and also initial part save that initial part we need it..
```

**Example :**

```
helm repo add grafana https://grafana.github.io/helm-charts &&
  helm repo update &&
  helm upgrade --install --atomic --timeout 300s grafana-k8s-monitoring grafana/k8s-monitoring \
    --namespace "monitoring" --create-namespace --values - <<'EOF'
```

Remove this above intial part and save it somewhere
Then Esc+wq! amd save the file

Now use the copied command just make some modification:
Remove that EOF part and instead write
--values values.yaml

**Example:**

```
helm repo add grafana https://grafana.github.io/helm-charts &&
  helm repo update &&
  helm upgrade --install --atomic --timeout 300s grafana-k8s-monitoring grafana/k8s-monitoring \
    --namespace "monitoring" --create-namespace --values values.yaml
```

Paste this command on VM u will get status deployed revision 1
It means it was a SUCESS

**To check:**

```
kubectl get pods -n monitoring
```

These are all should be running.....

Go to grafana cloud again..
And below u will get go to homepage click it..
Just refresh the page and boom..


<img width="757" height="332" alt="image" src="https://github.com/user-attachments/assets/08a66920-c588-4570-8483-d1cb38a7af03" />


Then explore the Home Page in Grafana Cloud


<img width="783" height="278" alt="image" src="https://github.com/user-attachments/assets/7098bfcc-698a-437a-9abd-09bb51f2b52e" />


Now I can monitor all the things through Grafana Cloud


<img width="914" height="426" alt="image" src="https://github.com/user-attachments/assets/b66b2f88-78a4-4191-a690-9bd311641ac9" />


You can play with multiple option that Grafan cloud has


<img width="928" height="275" alt="image" src="https://github.com/user-attachments/assets/bf662046-5153-45df-a193-ddb0b6af5beb" />


## Clean up

```
To delete the VM
Automatically Grafana Cloud stop the monitoring
```
