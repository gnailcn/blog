---
title: "First Post: A Guide to Building 'Wandering TideCatcher'"
date: 2024-07-25T11:00:00+08:00
categories: ["hugo"]
tags: ["hugo"]
summary: "This is not only the first post on this site but also a living document on how to add new posts and images—a blueprint for our future creative workflow."
draft: false
---

Hello, future me, and any friends who may happen to visit.

Welcome to the beginning of "Wandering TideCatcher." This space is envisioned as a basket to hold the "shells" and "stars" I pick up along the shores of knowledge and information. Today, I'm placing the first carefully chosen shell inside—a guide on how to create content here.

This post serves as both a memento and a guide, ensuring that every future act of creation is clear and efficient.

## I. The Starting Point: A Single Command

We don't create files manually. Instead, we use HUGO's elegant command-line tool. It's like a magic wand that prepares everything for us.

Open your terminal, navigate to the blog's root directory, and recite the spell:

```bash
# Format: hugo new content-type/YYYY/MM/your-post-slug/index.lang.md
hugo new posts/2024/07/a-new-journey/index.en.md
```

This command performs a bit of magic:

1.  It creates a folder named `a-new-journey` within the `content/posts/2024/07/` directory.
2.  Inside that folder, it creates an `index.en.md` file.
3.  It automatically populates this file with "identity information" (the Front Matter), including the title, date, and a crucial flag: `draft: true`. This flag marks it as a draft, visible in local previews but ignored during final deployment, which is very safe.

When we've finished writing and are ready for the world to see, we simply change `draft: true` to `draft: false`.

## II. Giving It Soul: Words and Images

A complete article is composed of both text and images. In our well-designed structure, managing them becomes incredibly simple.

### 1. Words

Below the file's "identity information" is where we let our words flow. It follows standard Markdown syntax—concise and powerful.

### 2. Images: An End to Chaos

This is the most beautiful part of our workflow. **Every article has its own dedicated folder**, which means all the images used in the article can be stored right alongside the article itself!

Let's say we're writing this `a-new-journey` post. Its directory structure looks like this:

```
content/
└── posts/
    └── 2024/
        └── 07/
            └── a-new-journey/          <-- The article's dedicated folder
                ├── index.en.md         <-- The article file itself
                └── journey-start.jpg   <-- Its companion image!
```

**How do you reference this image?**

In your `index.en.md` file, you just need to write the following, without any complex paths:

```markdown
![The Journey Begins](journey-start.jpg)
```

![The Journey Begins](journey-start.jpg)

It's that simple! The image and text are elegantly "bundled" together, making migration, backup, and management a worry-free experience.

## III. The Article's "ID Card": Front Matter

The area at the top of each article, wrapped in `---`, is its metadata. It determines how the article is categorized and displayed.

-   **`title`**: The title of the article.
-   **`date`**: The publication date, which determines its position in the archives.
-   **`categories`**: The category, usually a single, broad classification like `["Tech Notes"]` or `["Life Reflections"]`.
-   **`tags`**: Tags, which can be multiple and are used for more granular indexing, like `["Go", "Web", "Performance Tuning"]`.
-   **`summary`**: A short summary that will be displayed on the article list page.
-   **`draft`**: `false` means the article is published; `true` means it's a draft.

Carefully filling out this information will keep our knowledge base neat and organized.

## Conclusion

The creative process should be a joy, not a burden.

Start the journey with `hugo new`, place words and images in their dedicated folder, and finally, brush off the `draft` dust. This is the entire secret to recording every discovery here at "Wandering TideCatcher."

May this little basket grow fuller with each passing day.