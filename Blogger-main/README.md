# Blogger Project Setup Guide

Welcome to the **Blogger** project! Follow these steps to set up the project on your local machine and start contributing effectively.

---

### 1. Clone the Repository

Clone the project repository to your local machine. Open your terminal (Git Bash or any terminal you use) and run:

```bash
git clone https://github.com/Shivprasad-Solanke/Blogger.git
```

This will create a copy of the project folder on your computer.

---

### 2. Open the Project in VS Code

Navigate to the project folder and open it in Visual Studio Code:

```bash
cd Blogger
code .
```

Make sure you have the VS Code extensions for Python and Prettier installed.

---

### 3. Set Up Python Virtual Environment

Create a Python virtual environment to manage dependencies:

```bash
python -m venv env
```

Activate the virtual environment:

- **Windows**:
    ```bash
    .\env\Scripts\Activate
    ```

- **Mac/Linux**:
    ```bash
    source env/bin/activate
    ```

You should now see `(env)` in your terminal, indicating that the virtual environment is activated.

---

### 4. Install Project Dependencies

Install the required dependencies:

```bash
pip install -r requirements.txt
```

This will install FastAPI, Uvicorn, and other necessary packages.

---

### 5. Create a New Branch

To work independently and avoid conflicts, create a new branch for your task:

```bash
git checkout -b feature/<your-feature-name>
```

Example:
```bash
git checkout -b feature/dashboard
```

---

### 6. Start Your Work

Navigate to your assigned folder in the project structure (`home`, `dashboard`, `login_signup`, or `blog`) and work on your files:

- **Backend Work**:
  - Define routes in the respective `.py` files inside your folder.
  - For example, if working on the Dashboard, edit `dashboard.py` in `app/dashboard/`.

- **Frontend Work**:
  - Edit the HTML templates located in the `templates/` folder within your assigned module.
  - Add CSS and JavaScript files in `static/css/` and `static/js/` as needed.

---

### 7. Run the Development Server

After making changes, you can test your work by running the server:

```bash
uvicorn app.main:app --reload
```

- Open a browser and go to `http://127.0.0.1:8000` to view the application.
- Access the interactive API documentation at `http://127.0.0.1:8000/docs`.

---

### 8. Save and Commit Your Work

After completing your task:

1. **Stage your changes**:
   ```bash
   git add .
   ```

2. **Commit your changes** with a clear message:
   ```bash
   git commit -m "Implemented feature: Dashboard with Edit and Delete functionality"
   ```

3. **Push your branch** to the repository:
   ```bash
   git push -u origin feature/<your-feature-name>
   ```

---

### 9. Submit a Pull Request (PR)

1. Go to the [GitHub repository](https://github.com/Shivprasad-Solanke/Blogger).
2. Create a Pull Request (PR) to merge your branch into the `main` branch.
3. Add a clear description of the changes you made.
4. Request a review from other team members.

---

### 10. Pull Latest Changes

To stay updated with team contributions:

1. Switch to the `main` branch:
   ```bash
   git checkout main
   ```

2. Pull the latest updates:
   ```bash
   git pull origin main
   ```

3. Merge the latest changes into your branch:
   ```bash
   git checkout <your-branch-name>
   git merge main
   ```

Resolve any conflicts if necessary.

---

### Final Notes:
- Always activate your virtual environment before starting work.
- Coordinate with team members to ensure smooth integration of tasks.
- Commit changes often to avoid losing progress.
