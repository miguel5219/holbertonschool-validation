# Awesome API

## Prerequisites
go and make installed

## Lifecycle
build: Builds a website using gohugo on the dist folder
clean: Cleans the dist folder
post: Create a new blog post whose filename and title come from the environment variables POST_TITLE and POST_NAME
check:   Lints and check for dead links on markdowns using markdownlint-cli and markdown-link-check
validate:  Validates dist/index.html using W3C Hbtn validator
help: Shows this help
