# My Blog - GitHub Pages Static Site

A minimal, static blog site built with HTML and Tailwind CSS, designed to be hosted on GitHub Pages.

## 🚀 Quick Start: Deploy to GitHub Pages

### Option 1: User/Organization Site
1. Create a new repository named `<your-username>.github.io`
2. Copy all files from this folder to the repository
3. Push to the `main` branch
4. Your site will be live at `https://<your-username>.github.io`

### Option 2: Project Site
1. Create a new repository with any name (e.g., `my-blog`)
2. Copy all files from this folder to the repository
3. Go to **Settings → Pages → Source** and select `main` branch
4. Your site will be live at `https://<your-username>.github.io/<repo-name>`

---

## 📝 Adding a New Blog Post

### Step 1: Create the blog HTML file

1. Copy `blogs/example-blog.html` to a new file, e.g., `blogs/my-new-post.html`
2. Update the file with your content:

```html
<!-- Update the title -->
<title>Your Blog Title</title>

<!-- Update the heading and date -->
<h1 class="text-4xl mt-[57px] mb-3 font-serif">
  Your Blog Title
</h1>
<span class="text-sm text-gray-500">14th January, 2026</span>

<!-- Add your content -->
<p class="mt-4 font-serif text-lg">
  Your blog content goes here...
</p>
```

### Step 2: Add to the blog listing

Open `blogs/blog.html` and add a new entry at the top of the list:

```html
<ul class="list-none">
  <!-- Add your new entry here -->
  <a href="./my-new-post.html">
    <li class="flex justify-between items-center hover:underline underline-offset-4 py-3">
      <span class="text-gray-500 w-[40%]">14th January, 2026</span>
      <span class="w-full font-mono text-lg">Your Blog Title</span>
    </li>
  </a>
  <!-- Existing entries below -->
</ul>
```

### Step 3: Add images (optional)

1. Place images in `blogs/assets/`
2. Reference them in your blog post:

```html
<img src="./assets/your-image.png" alt="Description" class="mx-auto my-5 rounded-lg" />
```

---

## 📋 Adding a New Note

### Step 1: Create the note HTML file

1. Copy `notes/example-note.html` to a new file, e.g., `notes/my-note.html`
2. Update the content similar to blog posts

### Step 2: Add to the notes listing

Open `notes/notes.html` and add a new entry:

```html
<a href="./my-note.html">
  <li class="flex justify-between items-center hover:underline underline-offset-4 py-3">
    <span class="text-gray-500 w-[40%]">14th January, 2026</span>
    <span class="w-full font-mono text-lg">Your Note Title</span>
  </li>
</a>
```

### Linking to External Resources

You can also link directly to external resources without creating a local file:

```html
<a href="https://example.com/article">
  <li class="flex justify-between items-center hover:underline underline-offset-4 py-3">
    <span class="text-gray-500 w-[40%]">14th January, 2026</span>
    <span class="w-full font-mono text-lg">External Article Title</span>
  </li>
</a>
```

---

## 🎨 Customizing Your Site

### Change Site Name

Find and replace "My Blog" in all HTML files:
- `index.html` (line 6 for title, line 19 for header)
- `blogs/blog.html`
- `blogs/example-blog.html` (and any other blog posts)
- `notes/notes.html`
- `notes/example-note.html` (and any other notes)

### Change Author Name

Update the following in `index.html`:
```html
<h1 class="text-lg">
  Hi, myself <span class="font-semibold">Your Name</span>
</h1>
```

### Update Social Links

In `index.html`, update the social media links:
```html
<a href="https://twitter.com/yourusername" ...>Twitter</a>
<a href="https://github.com/yourusername" ...>Github</a>
<a href="https://linkedin.com/in/yourusername" ...>LinkedIn</a>
```

### Change Colors

The site uses Tailwind CSS classes. Main color classes used:
- `bg-orange-100` - Background color
- `bg-orange-200` - Code block background

To change, find and replace these classes in all files. For example, to use a different shade:
- `bg-slate-100` for a gray background
- `bg-blue-100` for a blue tint

---

## ➕ Adding MathJax (Mathematical Notation)

MathJax is already included in the templates. Use it like this:

### Inline Math
```html
<p>The famous equation \( E = mc^2 \) changed physics.</p>
```

### Block Math
```html
<div>
  \[ \int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2} \]
</div>
```

---

## 📁 Project Structure

```
my-blog/
├── index.html              # Home page
├── README.md               # This file
├── blogs/
│   ├── blog.html           # Blog listing page
│   ├── example-blog.html   # Example blog post (template)
│   └── assets/             # Blog images and assets
└── notes/
    ├── notes.html          # Notes listing page
    ├── example-note.html   # Example note (template)
    └── assets/             # Notes images and assets
```

---

## 🔧 Tips

1. **Keep filenames lowercase** with hyphens (e.g., `my-awesome-post.html`)
2. **Use relative paths** for all links to ensure portability
3. **Test locally** before pushing - just open `index.html` in a browser
4. **Commit and push** to see changes reflected on GitHub Pages (may take 1-2 minutes)

---

## 📄 License

Feel free to use and modify this template for your own blog!
