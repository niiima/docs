#Create documentation using git version control system
Having more than just source code in a repository is a very good thing, Documentation also should have a full history and the ability to revert to an earlier version if that becomes necessary. A version control system is perfect for this.


1. It groups all of your resources together and turns the project into a cohesive, centralized entity rather than a scattered collection of files. Contributors/employees know where to find everything, rather than sending "Where do I change the documentation for feature x?" emails.

1. You'll want to keep things organized. Have a system for separating the src from the images from the docs. You can always add a .gitignore to a directory to keep the repository and history clean. Because Git commits are file-based,* you can decouple source changes from documentation changes as strongly as you like.

1. Git is great for documentation versioning as long as it's text-based.

1. documentation should be versioned right alongside the code.

> The possible problem here is that it might be hard to set different access privileges for code and documentation in that case. And in many business cases people will need access to docs but not the source code, like marketing or BA departments. The answer is in Submodules.
> `git submodule add git@project:docs lib/docs`


