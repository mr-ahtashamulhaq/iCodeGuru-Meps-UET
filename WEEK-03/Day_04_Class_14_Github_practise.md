# Class 14 – GitHub Hands-On Practice

## 📝 Overview
Today’s session was a **practical class** where we learned to:
- Create a GitHub account.  
- Build our first repository.  
- Initialize repositories using Git.  
- Use basic Git commands (`add`, `commit`, `push`).  
- Upload code via **VS Code**.  
- Upload files by **drag-and-drop** directly on GitHub.  

---

## 1️⃣ Create a GitHub Account
1. Go to [GitHub.com](https://github.com).  
2. Click **Sign Up** → Enter your email, username, and password.  
3. Verify your email address.  
4. Add a **profile photo** and short bio for professionalism.  

---

## 2️⃣ Create Your First Repository
1. On GitHub, click the **“+” → New Repository** button.  
2. Enter a repository name (e.g., `first-repo`).  
3. Choose visibility: **Public** (recommended for beginners) or **Private**.  
4. Initialize with a **README.md** (optional but good practice).  
5. Click **Create Repository**.  

---

## 3️⃣ Initialize Repository (Local Setup)

```bash
# Create a new folder
mkdir first-repo
cd first-repo

# Initialize git
git init

# Link local folder with GitHub repo
git remote add origin https://github.com/username/first-repo.git
