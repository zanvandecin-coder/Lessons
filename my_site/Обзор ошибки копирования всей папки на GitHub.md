## Обзор ошибки копирования всей папки на GitHub

Yowza, that’s a lot of files. Try uploading fewer than 100 at a time.



This error occurs because GitHub's web interface drag-and-drop feature limits uploads to 100 files at a time. To upload more, use the **command line (`git add .`)**, **[GitHub Desktop](https://www.google.com/search?q=GitHub+Desktop&ved=2ahUKEwjjr86mt-yTAxWCEBAIHeYFO5kQgK4QegYIAQgAEAQ)**, or upload in smaller batches. It is also recommended to use a `.gitignore` file to exclude unnecessary folders like `node_modules`. 

Here are the best ways to resolve this issue:

- **Use Command Line Git (Recommended):** Instead of the browser, initialize a repository locally to bypass the limit.

  bash

```
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <URL>
git push -u origin main
```

**Use GitHub Desktop:** The GitHub Desktop app handles large numbers of files better than the web interface.

**Use `.gitignore`:** Create a `.gitignore` file to exclude unnecessary files (e.g., `node_modules/`, `bin/`, `obj/`, IDE settings) to reduce the file count.

**Upload in Batches:** If you must use the web interface, upload folders in chunks of fewer than 100 files. 

**Key Limitations:**

- **File Count:** Max 100 files via drag-and-drop.
- **File Size:** Individual files via web browser are limited to 25 MiB, or 100 MiB via command line.
- **Push Size:** Total push size is limited to 2 GiB.