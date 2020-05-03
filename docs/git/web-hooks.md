# Pre Commit Webhooks

1. We will be using __[gitmoji-cli](https://github.com/carloscuesta/gitmoji)__ webhook for commiting.
2. This would take care of all the rules we have read in [How to write good commit messages](/git/commit).

## Steps to use Webhooks

1. ### Installation
      **```npm i -g gitmoji-cli```** **:** This command will install gitmoji-cli globally on your machine
      
2. ### Usage
**```gitmoji --help```** **:** This command will show all the available commands

3. ### Commit

    This can we done in two ways

      1. #### Client
            
          **```git add .```**

          **```gitmoji -c```** **:** This command will start the interactive commit client and auto generates your commit
    
      2. #### Hook
        
          **```gitmoji -i```** **:** This command will intialize the commit as a commit hook

          **```git add .```**
          
          **```git commit```**