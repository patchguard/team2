-----------------------------------test step 1 start-------------------------------------------
```bash
git --version
git clone https://github.com/patchguard/teamworktest.git
cd teamworktest
git status
git branch --show-current
```
-----------------------------------test step 2 start-------------------------------------------

{branchname} is not a fixed name, please use owned branchname such as hwd1234 or other branch name you like. 
Each developer should use a separate branch for each task.

```bash
git switch main
git pull --ff-only origin main
git switch -c {branchname}
```

-----------------------------------test step 3 start-------------------------------------------

{dirname} is not the fixed folder name, you need to replace it as you owned folder. For example, hwd is one folder owned by user hwdsd2015

{branchname} is not branch name, please use you owned branch created at step 2.

```bash
mkdir {dirname}
cd {dirname}
echo "test" > README.md
git add README.md
git commit -m "docs: clarify contribution workflow"
git push -u origin {branchname}
```
