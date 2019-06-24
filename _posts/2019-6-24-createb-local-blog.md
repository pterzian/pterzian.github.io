Create folder `<github_user_name>.github.io/`

DDL & extract zip in folder [link to lanyon's github](https://github.com/poole/lanyon)

DDL & Install git from : [offical website](https://git-scm.com/download/win)

open powershell (Windows key + R key : type : `powershell` then press Enter key

go to your newly <github_user_name>.github.io/ folder : use `cd "path_to/folder_name`

type : `git init` to create a git repository.

Add all lanyon file to list of changes to apply and commit.

    git add *
    git commit

DDL & Install ruby <https://www.ruby-lang.org/en/>

come back to powershell, go to your folder path (for further use)

type : `gem install github-pages`

To make it work you have to modify the config file in two ways :

Open the config file by typing : `start wordpad .\_config.yml` or openning it with any text editor you prefer.

Comment this line : `#relative_permalinks: true` by adding the `#` at the beginning of the line.

Add these lines at the end of the document :

    #Gems
    gems : [jekyll-paginate]

Now all you have to do is to go back to the powershell at the same path and type

    jekyll build
    jekyll serve

It should print a bunch of message with your local adress at the end such as this : <http://127.0.0.1:4000/>. Go to that url adress through a web brower.

That should do the trick.
