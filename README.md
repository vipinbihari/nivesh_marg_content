# Blog Content Repository

This repository contains the content for the blog, separated from the main codebase for independent management.

## Structure

- **/posts/** - Contains all blog posts in MDX format
- **/uploads/** - Contains all images for blog posts

## Usage

This repository is designed to be used as a Git submodule in the main blog_cms repository.

## Workflow

1. Make changes to content in this repository
2. Commit and push changes
3. GitHub Actions will automatically trigger a build in the main repository

## Local Development

For local development, you can clone both repositories and set up symlinks:
```bash
# In your blog_cms directory
ln -s ../blog_content/posts ./src/content/posts
ln -s ../blog_content/uploads ./public/images/uploads
```
