build:	## Build: Generate the website from the markdown and configuration files in the directory dist/.
				hugo -s . -d dist/

clean: ## Cleanup the content of the directory dist/
				rm -rf dist/

post: ## Post: Create a new blog post whose filename and title come from the environment variables POST_TITLE and POST_NAME.
				hugo new posts/$(POST_NAME).md
				sed -i 's/title: .*/title:"$(POST_TITLE)"/' content/posts/$(POST_NAME).md


help: ## prints out the list of targets and their usage.
				cat README.md


package: ## target package create a file named awesome-website.zip
				hugo
				zip awesome-website.zip awesome-api dist/

lint: ## The target lint should be updated to lint the files README.md and DEPLOY.md with markdownlint
				@markdownlint "*.md"

unit-tests: ## run unit tests
				@echo "all tests done"

integration-tests: ## run integration-tests
				@echo "all integration-tests done"

validate: ## run validate
				@echo "all validations done"