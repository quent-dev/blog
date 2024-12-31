# Working with Github from the CLI

As I am starting to use Github more, I am trying to do everything from the command line.

Most of it is relatively easy, but I need to use the API to create the repo on Github first before being able to push the changes there.

The issue is that it requires authentication, ie. using a personal access token (PAT) and I don't want to have to copy paste it everytime from a password manager and we are trying to learn to do everything with as less steps as possible.

I figured I would create a Bash script who handles all the initial steps:

- Create a directory
- Add a README.MD file
- Initialize and the file to Git
- First commit
- Create the repo in github via API using our PAT
- Add remote origin
- Push to master

So I now created this script called ghnew and moved it to my PATH (I used /usr/bin in my case). I need to restart my terminal and test it out.

Of course it took another hour to have it work correctly:

- First, I learned that depending on your OS, your bash scripts need to start differently. Using a template I found on Substack, mine was not running because I was using the Windows convention which actually made it a DOS file and not a Unix file.

- Then, I discovered that my $reponame variable was not being evaluated inside of the single quotes so I need to change my script a little bit.

Now it is finally working, and I will be using this from now on when starting a new project to go faster.
