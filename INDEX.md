# Project Index — Linda Doe Twitter-Style Page

Quick-reference bookmark file. Jump directly to any file in this project.

---

## HTML

| File | Description |
|------|-------------|
| [tweet.html](tweet.html) | Main page — Twitter/X-style post from Linda Doe (@MomsWarning) about her daughter Jane's cosmetic surgery addiction. Contains the full thread with diary images, comment replies, sidebar nav, and lightbox markup. |

## CSS

| File | Description |
|------|-------------|
| [css/styles.css](css/styles.css) | All styles — reset, layout (3-column desktop: left sidebar, center feed, right sidebar), tweet/reply/thread components, image grids, action buttons, lightbox, responsive breakpoints (1300px, 1000px, 700px, 600px). |

## JavaScript

| File | Description |
|------|-------------|
| [js/lightbox.js](js/lightbox.js) | Lightbox image viewer — click `.grid-img` to open fullscreen, arrow keys / prev-next buttons to navigate, Escape or click backdrop to close. Tracks all `.grid-img` elements across all grids on the page. |

## Images — Diary Pages

| File | Description |
|------|-------------|
| [Diary_Images/1.png](Diary_Images/1.png) | Jane's first entry at 18 — the eyelid surgery (main tweet, grid position 1) |
| [Diary_Images/2.png](Diary_Images/2.png) | She thought it would stop there (main tweet, grid position 2) |
| [Diary_Images/3.png](Diary_Images/3.png) | The obsession began to grow (main tweet, grid position 3) |
| [Diary_Images/4.png](Diary_Images/4.png) | She couldn't recognize herself anymore (main tweet, grid position 4) |
| [Diary_Images/5.png](Diary_Images/5.png) | Writing about the pain after surgery (thread reply 1, grid position 1) |
| [Diary_Images/6.png](Diary_Images/6.png) | Hoping the next surgery would fix everything (thread reply 1, grid position 2) |
| [Diary_Images/7.png](Diary_Images/7.png) | She couldn't stop (thread reply 1, grid position 3) |
| [Diary_Images/8.png](Diary_Images/8.png) | She trusted the clinics (thread reply 2, grid position 1) |
| [Diary_Images/9.png](Diary_Images/9.png) | Each procedure was sold as routine (thread reply 2, grid position 2) |
| [Diary_Images/10.png](Diary_Images/10.png) | She kept going back (thread reply 2, grid position 3) |
| [Diary_Images/11.png](Diary_Images/11.png) | Jane's final diary entry (thread reply 3, single image) |

## Images — Profile Pictures

| File | Description |
|------|-------------|
| [Profile_Picture_Images/906c78c1baae6fcf84f75ca05631412e.png](Profile_Picture_Images/906c78c1baae6fcf84f75ca05631412e.png) | Linda Doe's avatar (OP — used in sidebar, main tweet, all thread replies, reply composer) |
| [Profile_Picture_Images/1054089f269ec953033c83145d25802a.png](Profile_Picture_Images/1054089f269ec953033c83145d25802a.png) | Dr. Sarah Kim's avatar (commenter 1) |
| [Profile_Picture_Images/519d2c4598073dd1409afb2d68157d61.png](Profile_Picture_Images/519d2c4598073dd1409afb2d68157d61.png) | maya's avatar (commenter 2) |
| [Profile_Picture_Images/cc032f64eece6f8a1035cd348cb40bed.png](Profile_Picture_Images/cc032f64eece6f8a1035cd348cb40bed.png) | James Morrison's avatar (commenter 4) |

---

## Page Structure (tweet.html)

```
.desktop
├── nav.sidebar-left          ← Navigation (Home, Explore, Notifications, Messages, etc.)
│   └── .nav-user             ← Linda Doe's profile card
├── main.center-col           ← Main content column
│   ├── .post-header          ← Sticky header with back arrow + "Post" title
│   ├── .tweet                ← Original post with text
│   │   ├── .image-grid.grid-4 ← Diary images 1–4 (2×2)
│   │   ├── .tweet-time-bar   ← Timestamp + view count
│   │   ├── .stats-bar        ← Reposts, Quotes, Likes, Bookmarks
│   │   └── .tweet-actions    ← Reply, Retweet, Like, Bookmark, Share
│   ├── .thread-tweet         ← OP reply 1: text + grid-3 (Diary_Images/5–7)
│   ├── .thread-tweet         ← OP reply 2: text + grid-3 (Diary_Images/8–10)
│   ├── .thread-tweet         ← OP reply 3: text + grid-1 (Diary_Images/11)
│   ├── .reply-composer       ← Reply input (readonly)
│   ├── .comments-divider     ← "Replies" label
│   └── .reply-tweet ×4       ← Comments (Dr. Sarah Kim, maya, The Guardian, James Morrison)
├── aside.sidebar-right       ← Search + trending topics + who to follow
└── .lightbox#lightbox        ← Fullscreen image viewer (hidden by default)
```
