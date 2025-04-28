Of course! 🚀
Here’s a full GCLOUD CLI Cheatsheet 📋 — clean, organized, and ready for you!

⸻

📚 GCLOUD CLI CHEATSHEET

🛠️ 1. Basic Setup

Task	Command
Install gcloud	Link
Update gcloud	gcloud components update
Initialize configuration	gcloud init
Authenticate	gcloud auth login
Set active project	gcloud config set project PROJECT_ID
View current config	gcloud config list



⸻

☁️ 2. Projects

Task	Command
List projects	gcloud projects list
Create new project	gcloud projects create PROJECT_ID
Set default project	gcloud config set project PROJECT_ID
Delete project	gcloud projects delete PROJECT_ID



⸻

🏢 3. Organizations and Folders

Task	Command
List organizations	gcloud organizations list
List folders	gcloud resource-manager folders list
Create a folder	gcloud resource-manager folders create --display-name="FOLDER_NAME" --organization=ORG_ID
Create folder under folder	gcloud resource-manager folders create --display-name="FOLDER_NAME" --parent=FOLDER_ID



⸻

👤 4. IAM (Identity and Access Management)

Task	Command
List IAM roles	gcloud iam roles list
Add role to user	gcloud projects add-iam-policy-binding PROJECT_ID --member='user:EMAIL' --role='roles/ROLE_NAME'
Remove role from user	gcloud projects remove-iam-policy-binding PROJECT_ID --member='user:EMAIL' --role='roles/ROLE_NAME'
View IAM policy	gcloud projects get-iam-policy PROJECT_ID



⸻

🖥️ 5. Compute Engine (VMs)

Task	Command
List instances	gcloud compute instances list
Create instance	gcloud compute instances create INSTANCE_NAME --zone=ZONE
SSH into instance	gcloud compute ssh INSTANCE_NAME --zone=ZONE
Start instance	gcloud compute instances start INSTANCE_NAME --zone=ZONE
Stop instance	gcloud compute instances stop INSTANCE_NAME --zone=ZONE
Delete instance	gcloud compute instances delete INSTANCE_NAME --zone=ZONE



⸻

🗃️ 6. Storage (GCS Buckets)

Task	Command
List buckets	gcloud storage buckets list
Create bucket	gcloud storage buckets create BUCKET_NAME --location=LOCATION
Upload file	gcloud storage cp FILE_PATH gs://BUCKET_NAME/
Download file	gcloud storage cp gs://BUCKET_NAME/FILE_PATH DESTINATION
Delete bucket	gcloud storage buckets delete BUCKET_NAME



⸻

📦 7. Cloud SQL

Task	Command
List instances	gcloud sql instances list
Create instance	gcloud sql instances create INSTANCE_NAME --database-version=MYSQL_8_0 --tier=db-f1-micro --region=us-central
Create user	gcloud sql users create USERNAME --instance=INSTANCE_NAME --password=PASSWORD
Connect to database	gcloud sql connect INSTANCE_NAME --user=USERNAME



⸻

🛡️ 8. Service Accounts

Task	Command
List service accounts	gcloud iam service-accounts list
Create service account	gcloud iam service-accounts create NAME --display-name="DISPLAY NAME"
Create and download key	gcloud iam service-accounts keys create key.json --iam-account=SA_NAME@PROJECT_ID.iam.gserviceaccount.com



⸻

🛠️ 9. Kubernetes (GKE)

Task	Command
List clusters	gcloud container clusters list
Create cluster	gcloud container clusters create CLUSTER_NAME --zone=ZONE
Get credentials for cluster	gcloud container clusters get-credentials CLUSTER_NAME --zone=ZONE
Deploy app	kubectl apply -f deployment.yaml



⸻

🌍 10. Networking

Task	Command
List VPC networks	gcloud compute networks list
Create VPC network	gcloud compute networks create NETWORK_NAME --subnet-mode=auto
List firewall rules	gcloud compute firewall-rules list
Create firewall rule	gcloud compute firewall-rules create RULE_NAME --allow tcp:80 --network=NETWORK_NAME



⸻

🎯 Bonus Tips

Shortcut	Meaning
--quiet	Skip all confirmation prompts
--project=PROJECT_ID	Specify project directly
--format=json/yaml/table	Change output format
gcloud help	Get help anytime

Example:

gcloud compute instances list --format=table



⸻

🚀 GCLOUD Quick Start Script (Optional)

gcloud init
gcloud auth login
gcloud config set project YOUR_PROJECT_ID
gcloud components update

🔥 Ready to use!

⸻

Would you also like me to create:
✅ A One-Page Printable Gcloud Cheatsheet PDF you can download? 📄🚀
👉 Just say “Yes, generate PDF!” 🎯
