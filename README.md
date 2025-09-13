## 🚀 GitHub Portfolio Refresher

### 📌 About the Project

This Python automation script **keeps your GitHub profile active** by automatically pushing a small “dummy” commit to a selected repository.
It updates a file with the **current timestamp**, pushes the commit, and ensures your **GitHub contributions graph stays green** — perfect for keeping your profile attractive to recruiters.


### ⚡ Features

* 📝 Auto-update a file (`refresh.md`) in your GitHub repo
* 🔄 Automatically commits & pushes changes
* 🟢 Keeps your GitHub profile activity **fresh & active**
* 🛡️ Safe setup — uses **local script with PAT or credentials**


### 🛠 Tech Stack

* Python 3
* Git CLI (local)
* subprocess (Python module)
* Optional: Windows Task Scheduler / cron for automation


### 📂 Project Setup

1. **Clone this repo**

   ```bash
   git clone https://github.com/cyberfortify/portfolio-refresher.git
   cd portfolio-refresher
   ```

2. **Create `refresh.md` file**

   ```bash
   echo "This file is used to keep the repo active." > refresh.md
   git add refresh.md
   git commit -m "Initial commit"
   git push
   ```

3. **Create Python script** (`github_refresher.py`)

   * Script updates `refresh.md` with current timestamp and pushes commit.
   * If script is outside repo, update `REPO_PATH` with full path to your repo.

4. **Install dependencies**

   ```bash
   # No extra pip packages required for basic script
   ```

5. **Run the script manually**

   ```bash
   python github_refresher.py
   ```


### 🔮 Optional Automation

* **Windows**: Use Task Scheduler to run script daily
* **Linux/macOS**: Use `cron` to schedule daily execution


### 📜 Future Enhancements

* Add multiple repo support in a single run
* Use GitHub API + Personal Access Token for password-less commits
* Add Telegram / email notifications on successful push


### ⚡ Output Example

* `refresh.md` will have lines like:

```
Last refreshed at 2025-09-13 19:23:45
```

* Commit message: `"Auto refresh at 2025-09-13 19:23:45"`
* GitHub contributions graph shows activity ✅


### 📜 License

This project is **open-source** and free to use under the MIT License.