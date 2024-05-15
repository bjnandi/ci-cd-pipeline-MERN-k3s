# CI/CD Pipeline for MERN App in Kubernetes (k3s) with GitHub Actions

### Step 1: Clone the repository in the local machine

```
git clone https://github.com/bjnandi/ci-cd-pipeline-MERN-k3s.git
```

### Step 2: Now, We need to fill in the secrets using GitHub Secrets that you can add to our GitHub repo. You can read GitHub Secrets for more details. Now we go to secrets and variables and set values.
```
Github > Repo Name > Settings > Secrets and variables > Action > Repository Secrets > New repository secret
```
<hr>

```
EC2_HOST: The public IP address of the bastion host EC2 instance, will look something like this “34.195.33.137”.
```
```
MASTER_NODE: The private IP address of the k8s-instance-master EC2 instance, will look something like this “10.0.1.222”.
```
```
EC2_USERNAME: The username of the EC2 instance, usually “ubuntu”.
```
```
SSH_PRIVATE_KEY: This will be our “.pem” file which will be used to login to the instance.
```
```
DOCKER_USERNAME: This will be the “username” of our docker hub you can see it when you go to the docker hub account profile. It will used to push the docker images on the docker hub.
```
```
DOCKER_PASSWORD: This is the “password” of your docker hub account.
```

### Step 3: Return to the “VS Code Editor” & edit or minor changes in the code or a UI file for the demo test then commit & push the code in the GitHub “main” branch for CI/CD testing in our app for now in the file:
```
client > src > components > Navbar.js file
```

Search “CRUD” text and replace it with “CRUD test” then commit and push it on the main branch.

## It takes some time to build, push, and deploy. Sometime later we saw our changes show in our app UI (http://bjtechlife.com) which works properly like inserting data

### Learn More Here
[Build an End-to-End CI/CD Pipeline for a MERN App in Kubernetes with Terraform using GitHub Actions & Ansible](https://medium.com/aws-in-plain-english/build-an-end-to-end-ci-cd-pipeline-for-mern-app-terraform-using-github-actions-with-ansible-d7686ccc8db1)

Happy coding! 💻✨
