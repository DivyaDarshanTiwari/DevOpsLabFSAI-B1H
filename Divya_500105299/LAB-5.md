# **LAB-5**

1.  Name- Divya Darshan Tiwari
2.  SAP- 500105299
3.  Roll No. - R2142220070
4.  Batch - B1H Full Stack AI

## **You added a Git submodule named `JS`, which clones the repository `https://github.com/DivyaDarshanTiwari/JS.git` into your project. Git warns that line endings in `.gitmodules` will change from LF to CRLF when modified on Windows.**

```bash
$ git submodule add https://github.com/DivyaDarshanTiwari/JS.git

```

## **You added a Git submodule (`JS`), which modified `.gitmodules`. The submodule is staged for commit, but `index.html` has unstaged changes.**

```bash
$ git status

```

## **You committed the submodule (`JS`), the `.gitmodules` file, and changes in `index.html`, linking the JS repository to your project.**

```bash
$ git add .
$ git commit -m "connected the files and added the js repo"

```

## **You successfully pushed your changes to the remote repository, including the JS submodule, `.gitmodules` file, and updates to `index.html`.**

```bash
$ git push

```

## **You initialized the submodule in your repository. This prepares Git to recognize and manage the submodule (`JS`) but does not update or fetch its content yet.**

```bash
$ git submodule init
$ ls

```

## **You added the `CSS` repository as a submodule in your project, updating the `.gitmodules` file. Now, commit the changes and push them to keep the submodule tracked. Run `git submodule update --init --recursive` if needed.**

```bash
$ git submodule add https://github.com/DivyaDarshanTiwari/CSS.git

```

## **You successfully added the `CSS` repository as a submodule and committed the changes. Next, push the commit to sync it with the remote repository.**

```bash
$ git submodule
$ git status
$ git commit -m "added the css repo as submodule"

```

## **`CSS` submodule addition has been successfully pushed to the remote repository.**

```bash
$ git push

```

## **Added `JS` and `CSS` repositories as submodules in the main HTML project, initializing and committing changes related to `.gitmodules`. Staged, committed, and pushed all modifications to the remote repository. Verified the status using `git status`, `git log`, and `git submodule` to ensure proper linking and updates. Successfully integrated and pushed all changes to GitHub.**

```bash
$ git log

```

---

# **New files added in `JS` and `CSS` repositories**

You have added new files in both `JS` and `CSS` submodules, and they have been updated in their respective repositories. Now, you need to update the submodules in the HTML module as well.

#### **Update the submodules in the HTML project**

```bash
$ git submodule update --remote --merge
$ git add .
$ git commit -m "Updated JS and CSS submodules in HTML module"
$ git push

```

This will fetch the latest changes from the `JS` and `CSS` repositories and update them in your main project.
