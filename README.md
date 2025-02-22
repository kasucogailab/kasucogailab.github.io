# KasuCogAI Lab Website

A quick guide for lab members to update and manage the website using GitHub and Markdown. (Site design based on [al-folio](https://github.com/alshedivat/al-folio).)

## Getting Started
Lab members should be able to:
- [Update their team profile](#how-to-update-or-add-a-team-profile)
- [Update the list of publications](#how-to-update-the-publication-list)
- [Add news posts](#how-to-add-news-posts)

To do this, you’ll need to understand:

### GitHub
GitHub is a version control platform that allows multiple people to work on the same project, track changes, and manage different versions.

### Markdown
This README.md file is written in Markdown, which allows for easy formatting:
- **Bold**: `**bold**`
- *Italics*: `*italics*`
- [Hyperlinks](http://www.example.com): `[text](URL)`

Refer to [this cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for more details.

### YAML
YAML is a structured data format used for defining content. Example:
```yaml
- name: John Doe
  position: Researcher
  email: john.doe@example.com
```
Ensure proper indentation with spaces (not tabs) and maintain consistency.

## How to Update (or Add) a Team Profile
### 1. Upload a Profile Picture
- Image size: 311px wide (JPEG/PNG)
- Name format: `team_firstname-lastname.jpg`
- Upload to `/assets/img/`

### 2. Edit Team Data
- Navigate to `/_data/members.yml`
- Click the edit (pencil) icon
- Add or modify an entry, following this format:
```yaml
- name: Jane Doe
  image: team_jane-doe.jpg
  position: AI Researcher
  email: jane.doe@example.com
  description: "Jane is an AI researcher focused on cognitive modeling."
```
- Click **Commit changes** to save.

## How to Update the Publication List
### 1. Get the Citation from PubMed
- Search for the paper at [pubmed.gov](https://pubmed.gov)
- Copy the citation in AMA format

### 2. Upload a Publication Image
- Save an image from the paper (185px wide preferred)
- Name format: `pubs_YEAR_keywords.png`
- Upload to `/assets/img/`

### 3. Edit Publication Data
- Navigate to `/_data/publications.yml`
- Click edit and add an entry following this format:
```yaml
- authors: "**Doe J**, **Smith A**."
  title: "AI and Cognitive Science."
  details: "Journal of AI Research, 2024."
  year: 2024
  image: pubs_2024_ai-cog.png
  pmid: 12345678
  doi: 10.1234/jair.5678
```
- Click **Commit changes**.

## How to Add News Posts
### 1. Create a Markdown File
- Navigate to `/_posts/`
- Click **Create new file**
- File format: `YYYY-MM-DD-title.md`

### 2. Add Content
Each post should start with:
```yaml
---
title: "New Research on AI"
author: Jane Doe
layout: post
group: news
---
```
Then, add the content in Markdown.

### 3. Commit the File
- Add a descriptive commit message
- Click **Commit changes**

After committing, refresh the website to see updates.
