### Intro: What is a patch file

- A git patch file is just a file that you can apply to a repository to get the changes / modifications / additions another developer did on his / her machine onto your local machine. This isn’t the only way to do that ofcourse but this is a viable method for a head/lead developer to check your code first before merging it into the repository’s main/master branch.

#### How to make a patch file

- Fire up a terminal, enter the repository via the terminal you opened (via the cd <repo_name_here> aka change directory command) and do the following commands (one line, one command)

        git add -A
        git config user.email "<your_email_address>"
        git config user.name "<your_name>"
        git commit -m 'Create Patch File'
        git format-patch -1 HEAD

  - The final command, i.e. git format-patch -1 HEAD, should produce the .patch file. 