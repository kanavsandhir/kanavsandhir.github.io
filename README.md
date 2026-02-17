You’re absolutely right 👌 — let’s make this a **complete start-to-finish documentation**, including how to create everything from scratch.

Below is the **final, structured, reusable guide**.

---

# 📘 Complete Documentation: Create a Public Resume Link Using GitHub Pages

Using: GitHub Pages

---

# 🎯 Goal

Host your resume publicly at:

```
https://yourusername.github.io/
```

Example:

```
https://kanavsandhir.github.io/
```

---

# 🟢 OPTION 1 — Easiest Method (10 Minutes Setup)

---

# 1️⃣ Step 1: Create a New Repository

1. Go to GitHub
2. Click **New Repository**
3. Repository name must be:

```
yourusername.github.io
```

⚠️ Must:

* Match your GitHub username exactly
* Be all lowercase
* Be public

Example:

If username is:

```
kanavsandhir
```

Repo name must be:

```
kanavsandhir.github.io
```

Select:

* ✅ Public
* ✅ Initialize with README (optional)

Click **Create repository**

---

# 2️⃣ Step 2: Upload Your Resume PDF

1. Click **Add file → Upload files**
2. Upload:

   ```
   Resume.pdf
   ```
3. Click **Commit changes**

---

# 3️⃣ Step 3: Create index.html

1. Click **Add file → Create new file**
2. Name it exactly:

```
index.html
```

3. Paste this:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Your Name - Resume</title>
</head>
<body style="text-align:center; font-family:Arial; margin-top:50px;">
  <h1>Your Name</h1>
  <p>Your Role</p>
  <a href="Resume.pdf" target="_blank">
    <button style="padding:10px 20px; font-size:16px;">
      View Resume
    </button>
  </a>
</body>
</html>
```

4. Commit changes.

---

# 4️⃣ Step 4: Enable GitHub Pages

Go to:

```
Repository → Settings → Pages
```

Under **Build and deployment**

Set:

```
Source: Deploy from branch
Branch: main
Folder: / (root)
```

Click Save.

Wait 1–3 minutes.

---

# 5️⃣ Step 5: Open Your Site

Open:

```
https://yourusername.github.io/
```

Done 🎉

---

# 🔴 Common 404 Issues & Fixes

If you see:

```
404 File not found
```

Check:

* Repo name matches username exactly
* All lowercase
* index.html exists
* index.html is in root (not inside folder)
* Branch is `main`
* Folder is `/ (root)`
* Hard refresh (Cmd + Shift + R)

---

# 📄 PDF Tab Shows Wrong Name (Like “John Doe’s CV”)

That is PDF metadata — not HTML title.

GitHub cannot change it.

---

## If Resume Created Using Word

Go to:

```
File → Info → Properties → Title
```

Change title → Save as new PDF → Upload again.

---

## If Resume Created Using LaTeX / RenderCV

Edit in source file:

```latex
\hypersetup{
    pdftitle={Your Name - Resume},
    pdfauthor={Your Name},
}
```

Regenerate PDF → Upload again.

---

# 🗑️ How to Delete File From Repo

1. Open file
2. Click 🗑️ Delete
3. Commit

GitHub Pages redeploys automatically.

---

# 🔄 Force Redeploy (If Changes Not Showing)

Edit `index.html`
Add a space
Commit

This forces rebuild.

---

# 🚀 Recommended Final Setup for Job Applications

Add both links in job applications:

```
Portfolio: https://yourusername.github.io/
Resume: https://yourusername.github.io/Resume.pdf
```

Looks more professional than only PDF upload.

---

# 🔥 Key Lessons Learned

* GitHub Pages is case-sensitive
* Repo name must match username exactly
* index.html must be in root
* PDF metadata is separate from HTML title
* Deployment may take 1–3 minutes
* Most 404 errors are naming/config issues

---

If you want next, I can:

* Create a reusable GitHub Pages starter template
* Convert this into a downloadable Markdown/PDF
* Or build you a clean modern portfolio template instead of basic HTML

You’ve officially learned how to deploy static sites now 👊
