## Command Line-Git-GitHub

### <u>Terminal Window</u>

### <u>Using the Command Line</u>
[Command Line Tutorial](http://generalassembly.github.io/prework/cl/#/) 

#### Typing cd (or cd ~) — a command for "change directory" — with no parameters takes us to our home directory:
cd
cd ~

#### Change the current directory (folder) (i.e., navigate to directory (folder) of choice):
cd ~/Desktop/

#### List directory (folder) contents:
ls

#### Make directories (folders):
mkdir example_folder

#### Change the current directory (folder) (i.e., navigate to new folder):
cd example_folder/

#### Print the current working directory:
pwd

#### Create a file (e.g., a text file; could be something different like Jupyter Notebook?????):
touch cat.txt
touch dog.txt
touch bird.txt
touch fish.txt

#### Remove directory (folder) entries (files):
rm cat.txt

#### Using Wildcards:
*List any file with "i" in the file name*
ls *i*

*Remove any file with "d"*
rm *d*

#### File pattern searcher (e.g., find all files with the word “the” inside):
grep -r “the” *

#### Find utility (e.g., find all Jupyter Notebook files within subdirectories of the current working directory):
find . | grep ipynb


### Introduction to Git
[Git Tutorial](https://try.github.io/levels/1/challenges/1) 

cd ~/Desktop
mkdir hello-world
cd hello-world

#### Create an empty Git repository or reinitialize an existing one:
git init
ls -A

#### Create a file:
touch a.txt

#### Show the working tree status:
git status

#### Add file contents to the index:
git add a.txt
git status

#### Record changes to the repository (-m for including log message):
git commit -m "Please remember this file at this time"

#### Show commit logs:
git log

#### Making and Cloning Repositories
#### Manage the set of tracked repositories ("remotes”):
git remote add origin https://github.com/tweichle/hello-world.git

#### *Pushing to GitHub*
#### Update remote refs along with associated objects (i.e., send files from local machine to remote repository on GitHub):
git push -u origin master

#### Create a README.md file:
nano README.md
git add README.md
git status
git commit -m "New README.md"
git push -u origin master

#### *Pulling from GitHub*
#### Fetch from and integrate with another repository or a local branch:
git pull origin master

#### Clone a repository into a new directory
git clone https://github.com/github-username/hello-world.git


#### These are common Git commands used in various situations:
git help

usage: git [--version] [--help] [-C <path>] [-c name=value]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

start a working area (see also: git help tutorial)
   clone      	Clone a repository into a new directory
   init       	Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        	Add file contents to the index
   mv         	Move or rename a file, a directory, or a symlink
   reset      	Reset current HEAD to the specified state
   rm         	Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect     	Use binary search to find the commit that introduced a bug
   grep       	Print lines matching a pattern
   log        	Show commit logs
   show       	Show various types of objects
   status     	Show the working tree status

grow, mark and tweak your common history
   branch     	List, create, or delete branches
   checkout   	Switch branches or restore working tree files
   commit     	Record changes to the repository
   diff     		Show changes between commits, commit and working tree, etc
   merge      	Join two or more development histories together
   rebase     	Reapply commits on top of another base tip
   tag          Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      	Download objects and refs from another repository
   pull       	Fetch from and integrate with another repository or a local branch
   push       	Update remote refs along with associated objects

git help -a

'git help -a' and 'git help -g' list available subcommands and some concept guides

available git commands:
  add                       			merge-ours
  add--interactive          		  merge-recursive
  am                        			merge-resolve
  annotate                  			merge-subtree
  apply                     			merge-tree
  archive                   			mergetool
  bisect                    			mktag
  bisect--helper            			mktree
  blame                     			mv
  branch                    			name-rev
  bundle                    			notes
  cat-file                  			p4
  check-attr                			pack-objects
  check-ignore              			pack-redundant
  check-mailmap             		  pack-refs
  check-ref-format          		  patch-id
  checkout                  			prune
  checkout-index            		  prune-packed
  cherry                    			pull
  cherry-pick               			push
  citool                    			quiltimport
  clean                     			read-tree
  clone                     			ebase
  column                    			rebase--helper
  commit                    			receive-pack
  commit-tree            			    reflog
  config                    			remote
  count-objects             			remote-ext
  credential                			remote-fd
  credential-cache          		  remote-ftp
  credential-cache--daemon  	    remote-ftps
  credential-osxkeychain    		  remote-http
  credential-store          		  remote-https
  daemon                    			remote-testsvn
  describe                  			repack
  diff                      			replace
  diff-files                			request-pull
  diff-index                			rerere
  diff-tree                 			reset
  difftool                  			rev-list
  difftool--helper          			rev-parse
  fast-export               			revert
  fast-import               			rm
  fetch                     			send-email
  fetch-pack                			send-pack
  filter-branch             			sh-i18n--envsubst
  fmt-merge-msg             		  shell
  for-each-ref              			shortlog
  format-patch              			show
  fsck                      			show-branch
  fsck-objects              			show-index
  gc                        			show-ref
  get-tar-commit-id         		  stage
  grep                      			stash
  gui--askpass              			status
  hash-object               			stripspace
  help                      			submodule
  http-backend              		  submodule--helper
  http-fetch                			subtree
  http-push                 			svn
  imap-send                 			symbolic-ref
  index-pack                			tag
  init                      			unpack-file
  init-db                   			unpack-objects
  instaweb                  			update-index
  interpret-trailers        			update-ref
  log                       			update-server-info
  ls-files                  			upload-archive
  ls-remote                 			upload-pack
  ls-tree                   			var
  mailinfo                  			verify-commit
  mailsplit                 			verify-pack
  merge                     			verify-tag
  merge-base                			web--browse
  merge-file                			whatchanged
  merge-index               			worktree
  merge-octopus             		  write-tree
  merge-one-file
