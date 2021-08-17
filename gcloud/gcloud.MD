
# My gcloud most used commands:

### Auth
```
gcloud auth login
```

### List instances
```
gcloud compute instances list
```

### List subnets
```
gcloud compute networks subnets list
```

### Watch things
```
watch "gcloud compute instances list | grep <instance name>"
```

### Create local credentials file from service account
```
gcloud iam service-accounts keys create my_credential.json --iam-account=[account]
```

### Get permissions (policies) from project id
```
gcloud projects get-iam-policy <project_id>
```

### List permissions of role in a organization
```
gcloud iam roles describe <role_id_only_without_roles_slash> --organization <org_id>
``` 

### Add permission to Role
```
gcloud iam roles update <role> --add-permissions=container.clusters.delete,container.clusters.list --organization <org_id>
```
### Associate a role to a project
```
gcloud projects add-iam-policy-binding someprojecthere --member "serviceAccount:gcpcmdlineuser@someproject.iam.gserviceaccount.com" --role "roles/owner"
```

### Get lis of members/service account and policies 
```
gcloud projects get-iam-policy <project>
```

### Add member of Org to project
```
gcloud projects add-iam-policy-binding <project> --member "serviceAccount:<sa..>" --role organizations/<org_id>/roles/<role>
```

