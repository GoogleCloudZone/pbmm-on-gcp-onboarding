# pbmm-on-gcp-onboarding
- https://github.com/GoogleCloudZone/pbmm-on-gcp-onboarding/wiki/
GCP Secure Landing Zone - based on original TEF V4 copy


# Deployment
## gcp-bootstrap
```
Welcome to Cloud Shell! Type "help" to get started, or type "gemini" to try prompting with Gemini CLI.
To set your Cloud Platform project in this session use `gcloud config set project [PROJECT_ID]`.
You can view your projects by running `gcloud projects list`.
michael@cloudshell:~$ gcloud config set project lz-ado-xyz-boot-ot
Updated property [core/project].
michael@cloudshell:~ (lz-ado-xyz-boot-ot)$ cd ado/gcp-bootstrap/envs/shared/
michael@cloudshell:~/ado/gcp-bootstrap/envs/shared (lz-ado-xyz-boot-ot)$ eval `ssh-agent`
Agent pid 1599
michael@cloudshell:~/ado/gcp-bootstrap/envs/shared (lz-ado-xyz-boot-ot)$ ssh-add ~/.ssh/ado-xyz-oldev-from-ot
Identity added: /home/michael/.ssh/ado-xyz-oldev-from-ot (michael@obrienlabs.dev)
michael@cloudshell:~/ado/gcp-bootstrap/envs/shared (lz-ado-xyz-boot-ot)$ terraform init
Initializing the backend...
Initializing modules...
Initializing provider plugins...
- Reusing previous version of hashicorp/random from the dependency lock file
- Reusing previous version of hashicorp/google-beta from the dependency lock file
- Reusing previous version of hashicorp/null from the dependency lock file
- Reusing previous version of hashicorp/time from the dependency lock file
- Reusing previous version of hashicorp/google from the dependency lock file
- Using previously-installed hashicorp/time v0.13.1
- Using previously-installed hashicorp/google v5.45.2
- Using previously-installed hashicorp/random v3.7.2
- Using previously-installed hashicorp/google-beta v5.45.2
- Using previously-installed hashicorp/null v3.2.4

Terraform has been successfully initialized!
```
