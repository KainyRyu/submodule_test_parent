# submodule_test_parent
To see how submodule work with the main project.

### To add submodule : 
`git submodule add submoduleURL submodule_name(optional)`

### To update submodue : 
`git submodule update --remote`

### Check if upstream has a change : 
`git submodule update --remote --merge`

Or do `git push --recurse-submodules=check`

-> "check" basically makes `push` to be failed if submodule's local commit hasn't pushed.

`git push --recurse-submodules=on-demand` will makes git to push the commit in submodule before push the main project.

If you want to this command line every time you push : `git config push.recurseSubmodules on-demand`

