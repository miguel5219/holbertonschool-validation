# Prerequisites

Before you begin this tutorial you must:

    Install Hugo
    Install Git

## Requirements

    Use the theme “ananke” for the website by following the section Note for
    non-git users at the Step 3
    Usage of Git Submodules is prohibited: there should be no file .gitmodules
    The website title should be “Awesome Inc.”
    The contents consists in a single blog post which title should be
    “Welcome to Awesome Inc.”, stored in a file named welcome.md
    All of the website’s source code is stored under a directory named
    module1_task0
    The command line hugo in version 0.84.0 must be used
    The website is expected to be generated into the directory
    module1_task0/dist/
    The directory module1_task0/dist/ must not be committed
    (it should be absent from the repository) Here is a simple example of the
    expected generation process:

## Lifecycle

lifecycle is generally staying the same. In this project, you will start to
define this lifecycle via the following steps::

        build: Build: Generate the website from the markdown and configuration
        files in the directory dist/

        clean: Cleanup the content of the directory dist/

        post: Post: Create a new blog post whose filename and title come from
        the environment variables POST_TITLE and

        help: prints out the list of targets and their usage.
