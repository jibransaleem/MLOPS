dvc remote add -d myremote s3
-d stands for default

Makes this remote the default remote

After this, you don’t need to specify remote name again


Initialize DVC
dvc init
✔ Initializes DVC in a Git repo
✔ Creates .dvc/ folder

dvc add data.csv
✔ Creates data.csv.dvc
✔ Data not stored in Git

dvc status

dvc checkout
✔ Restores data for current Git commit

Push data to remote
dvc push

Pull data from remote
dvc pull

Remove tracked file
dvc remove data.csv.dvc

Show remotes
dvc remote list

Show DVC files
dvc list .

Init → Add → Commit → Push → Repro → Compare
dvc init
dvc add
git commit
dvc push
dvc repro
dvc metrics show
