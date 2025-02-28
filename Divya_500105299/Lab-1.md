# LAB1

### Why Do We Use Git?

Git is a **version control system** that’s super helpful for developers. It lets you keep track of changes in your code, work with others more smoothly, and manage different versions of a project. Here’s what it can do:

- **Track Changes**: You can see a history of every change made to the code.
- **Collaborate**: Multiple people can work on the same project without stepping on each other’s toes.
- **Branching & Merging**: You can create separate branches to work on new features or fixes without messing up the main code.
- **Backup & Restore**: If something goes wrong, you can always go back to a previous version of your project.

---

### How to Create a Repository on GitHub and Clone It

#### **Step 1: Create a Repository on GitHub**

1. Head over to [GitHub](https://github.com) and log in to your account.
2. Click the **"+"** icon in the top right corner and select **"New repository"**.
3. Give your repository a name (e.g., `my-project`).
4. Choose whether you want it to be **Public** (anyone can see it) or **Private** (only you and collaborators can access it).
5. (Optional) You can add a README file to describe your project.
6. Click **"Create repository"** to finish.

---

#### **Step 2: Clone the Repository to Your Computer**

1. Once your repository is created, go to its main page on GitHub.
2. Click the **"Code"** button and copy the URL (you can use either HTTPS or SSH, depending on your preference).
3. Open your **Terminal** (if you’re on Mac/Linux) or **Command Prompt/Git Bash** (if you’re on Windows).
4. Run the following command to clone the repository to your local machine:

   ```bash
   git clone <repository-url>
   ```

   For example:

   ```bash
   git clone https://github.com/your-username/my-project.git
   ```

5. Once the cloning is done, navigate into the project folder:

   ```bash
   cd my-project
   ```

How you have created your first repo
