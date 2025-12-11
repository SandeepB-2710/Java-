# create a new repository on the command line

```
echo "# Java-Classes" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin repo link.git
git push -u origin main
```


# push an existing repository from the command line

```
git remote add origin repo link.git
git branch -M main
git push -u origin main
```


1
```git init```

This turns your current folder into a Git repository. It tells the computer, "Start tracking changes in this folder."

It’s like buying a brand-new, empty diary to start writing your project history.  




2
 ```git add .```

This adds all the files in the folder to a "staging area," getting them ready to be saved. The . means "all files here."
   
Analogy: You are gathering all your items and putting them into a box, but you haven't sealed the box yet.  

3
```git commit -m "Initial commit"```

This permanently saves the changes you just "added." The message in quotes ("Initial commit") is a note describing what you did.
   
You tape the box shut and put a label on it that says "My first set of items." Now it's safe and recorded.  




4
```git remote add origin your URL.git```

This connects your local folder on your computer to a specific place on the internet (GitHub). "Origin" is just a nickname for that online address.

You are writing the destination address on the package so the post office knows where to send it.  




5
```git branch -M main```  

This renames your current working branch to "main." It’s the standard name for the primary version of your code.
   
You are just renaming your workspace from "master" (the old default) to "main" (the new standard name).  




6
```git push -u origin main```  

Simple Explanation: This uploads your saved changes (commits) from your computer to the online repository (GitHub).

Analogy: You finally hand the package over to the post office (Internet) to be delivered to the destination address (GitHub).  

