# EducationalAdventure
Educational adventure game for children at elementary level schools

**CURRENT UNITY VERSION: 2018.3.5f1** -> You can get it from unity hub archive

**HOW TO CONTRIBUTE**

1. Create a new branch for your feature or issue
2. Checkout your new branch
3. Write code and commit it to your branch
4. If you finished, open a pull request and wait for review 

**MERGING TOOLS**
It is important to use UnityYAMLMerge to avoid many merge conflicts with .unity and .asset files
Unity provides us with that tool so no need for additional downloads. To add such a capability 
to your git toolchain you will need to create .gitconfig file in your local repository, then add the 
following lines:
```
[merge]
tool = unityyamlmerge

[mergetool "unityyamlmerge"]
trustExitCode = false
cmd = 'Path to UnityYAMLMerge.exe' merge -p "$BASE" "$REMOTE" "$LOCAL" "$MERGED"
```
UnityYAMLMerge.exe is usually located in:  'Your Unity Install Dir'/Unity/Editor/Data/Tools/
For windows users: It is important to note the direction of slashes, use forward slashes in .gitconfig
to avoid potential problems.
