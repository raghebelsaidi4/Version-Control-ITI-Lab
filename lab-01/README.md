# Git Lab Solution

This repository contains solutions to the Git lab exercise.

## Steps to Complete the Lab

### 1. Install Git
- Download and install Git from [git-scm.com](https://git-scm.com/downloads).
- Verify installation with:
  ```sh
  git --version
  ```

### 2. Create a GitHub Account
- Sign up at [GitHub](https://github.com/).
- Confirm your email and log in.

### 3. Accept Contribution Invitation & Clone Repository
- Accept the GitHub invitation from Gmail.
- Clone the repository:
  ```sh
  git clone <repository_url>
  cd <repository_name>
  ```

### 4. Edit the Repository & Push Changes
- Create a new file with your name and email:
  ```sh
  echo "Your Name: <Your Name>" > my_info.txt
  echo "Your Email: <Your Email>" >> my_info.txt
  ```
- Stage, commit, and push changes:
  ```sh
  git add my_info.txt
  git commit -m "Added my_info.txt with name and email"
  git push origin main
  ```

### 5. Create a New Local & Remote Repository
- Create a new repository on GitHub.
- Initialize a local repository:
  ```sh
  mkdir my_new_repo
  cd my_new_repo
  git init
  ```
- Create a file with your full name:
  ```sh
  echo "Full Name: <Your Full Name>" > my_name.txt
  ```
- Add, commit, and push:
  ```sh
  git add my_name.txt
  git commit -m "Added my_name.txt with full name"
  git remote add origin <repository_url>
  git branch -M main
  git push -u origin main
  ```

### 6. Invite User to the Repository
- Go to the repository on GitHub.
- Navigate to "Settings" → "Manage access" → "Invite a collaborator".
- Enter **ahmedibrahem22322@gmail.com** and send the invitation.

### 7. Update README.md
- Create a `README.md` file:
  ```sh
  echo "# Git Lab Solution" > README.md
  echo "This repository contains solutions to the Git lab exercise." >> README.md
  ```
- Commit and push:
  ```sh
  git add README.md
  git commit -m "Added README.md with lab instructions"
  git push origin main
  ```

