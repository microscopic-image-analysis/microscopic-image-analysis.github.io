# Microscopic Image Analysis Website

This repository contains the source for https://microscopic-image-analysis.github.io

## How to maintain the website

1. Update the files `_includes/about.html` and `_includes/contact.html` for the
   landing page.
2. Write news in the `_posts` directory following the file format `yyyy-mm-dd-title.md`
   with the following form:
   ```md
   ---
   layout: post
   title: "Post title"
   ---

   Post content
   ```
3. One markdown file per group member in the `_team` directory:
   ```md
   ---
   name: "Your name goes here"
   role: "What you role is (Group leader, Postdoc, PhD student, Research assistant, Student, ...)"
   ordering: 1
   imgpath: "/assets/your-image.jpg"
   teaser: "A very short description of what you do"
   layout: member
   ---

   Arbitary content describing yourself.
   Use
   {% include publication-list.html name="your name" %}
   to include a personalised publication list.
   ```
   For the `ordering` key, pick a number corresponding to your role:
   | `role`             | `ordering` |
   | ------------------ | ---------- |
   | Group leader       | 1          |
   | Postdoc            | 2          |
   | PhD student        | 3          |
   | Research assistant | 4          |
   | Student            | 5          |
   
4. One markdown file per lecture in the `_lectures` directory:
   ```md
   ---
   name: "Name of the lecture"
   state: planned # see explanation below
   when: "When this lecture takes place, e.g. Summer 2023"
   layout: lecture
   ---

   Arbitraty content describing this lecture
   ```
   Set `state: current`, `state: planned`, or `state: old` in the frontmatter
   depending on if the lecture is currently held, planned for the future, or was
   held in the past.
5. One markdown file per research project in the `_projects` directory:
   ```md
   ---
   name: "Name of the project"
   state: current # see explanation below
   when: "Over which time span this project runs/ran"
   layout: project
   ---

   Arbitrary content describing this project
   ```
   Set `state: current` or `state: old` in the frontmatter depending on if the
   project is still active or already completed.
6. One markdown file per publication in the `_publications` directory:
   ```md
   ---
   involved:
      - "Name of first involved member"
      - "Name of second involved member"
   ---

   Formatted description of the paper (title, journal, year, authors, ...)
   ```
   Use a `yyyy-mm-dd-name.md` naming scheme for the file to ensure proper sorting
   in the publication list.