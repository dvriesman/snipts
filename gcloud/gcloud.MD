
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



