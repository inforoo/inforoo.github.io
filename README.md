# Description

Mathsalon website.  
Static website, using HTML + CSS

## Requirements

    "bootstrap": "5.0.1",
    "popper.js": "1.16.1" (popovers are not used in a project yet)

## Style

    <link rel="stylesheet" href="./css/bootstrap.min.css">
    <link rel="stylesheet" href="./css/style.css">

You can override the default styles of Bootstrap elements using two possible methods. The first way — using CSS overrides — applies to sites using BootstrapCDN or the pre-compiled versions of Bootstrap. The second — using SASS variables — applies to sites using the source code version of Bootstrap.

We prefer the first way here — using CSS overrides — in style.css;  

- We haven't extra dependency from SASS compilation making the code more self-sufficient.
- Menu actions (like :hover, :focus) isn't possible to change using just Bootstrap SASS variables. 

You can make as many changes as needed to transform your Bootstrap site. Just make sure to use CSS selectors that are as specific as — or more specific than — those in the bootstrap.css file.

## Git setup with key authentication (reminder)
1. create ssh keys, copy locally to `~/.ssh`
2. copy ssh public key to github (github account settings menu)
3. add github connection to `~/.ssh/config`
    
       Host [connection name here]
           User git
           Hostname github.com
           PreferredAuthentications publickey
           IdentityFile ~/.ssh/[private key name here]

4. create local repository

       git init
       
   or clone it (https protocol)
       
       git clone https://github.com/inforoo/inforoo.github.io.git
       
   then add remote host (ssh protocol)
       
       git remote add origin [connection name here]:inforoo/inforoo.github.io.git
       
5. standard workflow
    
       git add --all
       git commit -m "initial commit"
       git push -u origin master
    
 


