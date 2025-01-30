

# Lab 2 Solution

### 1. Create a new project locally and push it to the remote repository
```sh
mkdir new_project
cd new_project
git init
echo "New project" > project.txt
git add .
git commit -m "Initial commit"
git remote add origin <repository_url>
git push -u origin main
```

### 2. Create two branches (dev & test) and add files
```sh
git branch dev
git branch test
git checkout dev
echo "Development branch file" > dev_file.txt
git add dev_file.txt
git commit -m "Added dev_file.txt"
git push origin dev

git checkout test
echo "Test branch file" > test_file.txt
git add test_file.txt
git commit -m "Added test_file.txt"
git push origin test
```

### 3. Merge branches into master and push
```sh
git checkout master
git merge dev
git merge test
git push origin master
```

### 4. Remove the dev branch locally and remotely
```sh
git branch -d dev
git push origin --delete dev
```

### 5. Create an annotated tag (v1.7) and push it
```sh
git tag -a v1.7 -m "Version 1.7"
git push origin v1.7
```

### 6. List tags
```sh
git tag
```

### 7. Delete a tag locally and remotely
```sh
git tag -d v1.7
git push origin --delete v1.7
```

### 8. Add an image in README.md
To add an image, insert the following line into `README.md`:
```md
![Git Logo](https://git-scm.com/images/logos/downloads/Git-Logo-2Color.png)
```

