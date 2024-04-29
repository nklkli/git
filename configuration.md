# GLOBAL CONFIGURATION

Open global configuration file:

    git config --global -e

Configure `Visual Studio Code` as Git's default text editor, diff and merge tool:

<pre>        
[core]
    editor = code --wait
    autocrlf = true
[diff]
    tool = default-difftool
[difftool "default-difftool"]
    cmd = code --wait --diff $LOCAL $REMOTE
[merge]
    tool = code
[mergetool "code"]
    cmd = code --wait --merge $REMOTE $LOCAL $BASE $MERGED
[difftool]
    prompt = false
</pre>
