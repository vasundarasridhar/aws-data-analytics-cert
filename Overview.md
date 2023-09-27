**Exam Overview**

| Domain                           | % of Exam     |
|----------------------------------|---------------|
| 1. Collection                    |    18%        |
| 2. Storage and Data Management   |    22%        |
| 3. Processing                    |    18%        |
| 4. Analysis and Visualization    |    18%        |
| 5. Security                      |    18%        |


**AWs Cloudshell commands:**
we can upload one file at a time from local to directory, size is limited to 1GB. We can also download the files present in the Actions tab.For download, get the path and put it in the requested place.
- **pwd** - shows where the path is 
- **ls**- lists the files in the directory
- **df** -h - this shows us the file system(storage available and stuff)
- **echo $SHELL** - It gives Bash which is the default environment.We can also use other shells like zsh and powershell(pwsh is the command)
- **exit** - exits the shell.
- **aws s3api create-bucket --bucket your-bucket-name --region us-east-1**: Create a bucket from command line
- **aws s3 ls | wc -l** : count the number of buckets
- **Synchronize the buckets**:
- #yourbucketname
- aws s3 sync . s3://yourbucketname
