GIT
===

## Acknowledgements

Git = SCM ~= SVN ~= CVS ~= Mercurial (hg) ~= Perforce ~= ...

Copy Paste / Errores de codigo duplicado / Merge errors


Ejemplo: Rails app

Jose
editar: Gemfile
  add gem 'devise'

Richard
editar: Gemfile
  add gem 'compass'

    Gemfile:

    source 'https://rubygems.org'

    ruby '2.0.0'

    gem 'rails', '~ 4.0'
    gem 'compass'


SCM = SOLUCION!

Workflow (Convenciones)

Ejemplo:

GIT:

  1. Repositorio por cada developer
    - .git
  2. Entorno de trabajo (Workspace)
    - Carpeta del proyecto - .git

Ejemplo

total 11792
drwxr-xr-x  41 jfgomez86  staff     1394 May 13 16:14 .
drwxr-xr-x  50 jfgomez86  staff     1700 Apr 15 20:53 ..
-rw-r--r--@  1 jfgomez86  staff     6148 Nov 25 10:25 .DS_Store
drwxr-xr-x  17 jfgomez86  staff      578 May 13 16:12 .git
-rw-r--r--   1 jfgomez86  staff      246 Mar 18 20:07 .gitignore
-rw-r--r--   1 jfgomez86  staff      113 May 10  2013 .powrc
-rw-r--r--   1 jfgomez86  staff       15 May  9  2013 .rspec
-rw-r--r--   1 jfgomez86  staff       16 May 14  2013 .ruby-gemset
-rw-r--r--   1 jfgomez86  staff       16 Mar 18 20:07 .ruby-version
-rw-r--r--   1 jfgomez86  staff      312 May  9  2013 .watchr
-rw-r--r--   1 jfgomez86  staff      172 May  9  2013 Capfile
-rw-r--r--   1 jfgomez86  staff     3414 Mar 18 20:07 Gemfile
-rw-r--r--   1 jfgomez86  staff    16986 Mar 18 20:07 Gemfile.lock
-rw-r--r--   1 jfgomez86  staff      532 May  9  2013 Guardfile
-rw-r--r--   1 jfgomez86  staff    10359 May  9  2013 LICENSE
-rw-r--r--   1 jfgomez86  staff      543 Mar 18 20:07 Procfile
-rw-r--r--   1 jfgomez86  staff      178 Mar 18 20:07 Procfile.dev
-rw-r--r--   1 jfgomez86  staff     2313 Mar 18 20:07 README.md
-rw-r--r--   1 jfgomez86  staff      295 May  9  2013 Rakefile
drwxr-xr-x  20 jfgomez86  staff      680 Mar 18 20:07 app
drwxr-xr-x   3 jfgomez86  staff      102 May  9  2013 autotest
drwxr-xr-x   3 jfgomez86  staff      102 May  9  2013 bin
drwxr-xr-x   7 jfgomez86  staff      238 Mar 18 20:07 cert
-rw-r--r--   1 jfgomez86  staff       41 Mar 18 20:07 circle.yml
drwxr-xr-x  19 jfgomez86  staff      646 Mar 18 20:07 config
-rw-r--r--   1 jfgomez86  staff      163 May  9  2013 config.ru
drwxr-xr-x   7 jfgomez86  staff      238 Mar 18 20:07 db
drwxr-xr-x   3 jfgomez86  staff      102 May  9  2013 doc
drwxr-xr-x   4 jfgomez86  staff      136 May  9  2013 gamlet
-rw-r--r--   1 jfgomez86  staff     1732 May  9  2013 gamlet.zip
-rw-r--r--   1 jfgomez86  staff       91 May 13 16:14 git.course.md
-rw-r--r--   1 jfgomez86  staff  5924899 Jan 31 11:16 latest.dump
drwxr-xr-x  31 jfgomez86  staff     1054 Mar 18 20:07 lib
drwxr-xr-x   4 jfgomez86  staff      136 May 10  2013 log
drwxr-xr-x  32 jfgomez86  staff     1088 Mar 18 20:07 public
-rw-r--r--   1 jfgomez86  staff        0 May  9  2013 restart
drwxr-xr-x   3 jfgomez86  staff      102 May  9  2013 script
drwxr-xr-x  21 jfgomez86  staff      714 Mar 18 20:07 spec
-rw-r--r--   1 jfgomez86  staff        0 May  9  2013 teammate
drwxr-xr-x   4 jfgomez86  staff      136 May 10  2013 tmp
drwxr-xr-x   4 jfgomez86  staff      136 May  9  2013 vendor


Trbajando con Git:

`git`

usage: git [--version] [--help] [-C <path>] [-c name=value]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p|--paginate|--no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

The most commonly used git commands are:
   add        Add file contents to the index
   bisect     Find by binary search the change that introduced a bug
   branch     List, create, or delete branches
   checkout   Checkout a branch or paths to the working tree
   clone      Clone a repository into a new directory
   commit     Record changes to the repository
   diff       Show changes between commits, commit and working tree, etc
   fetch      Download objects and refs from another repository
   grep       Print lines matching a pattern
   init       Create an empty Git repository or reinitialize an existing one
   log        Show commit logs
   merge      Join two or more development histories together
   mv         Move or rename a file, a directory, or a symlink
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects
   rebase     Forward-port local commits to the updated upstream head
   reset      Reset current HEAD to the specified state
   rm         Remove files from the working tree and from the index
   show       Show various types of objects
   status     Show the working tree status
   tag        Create, list, delete or verify a tag object signed with GPG

'git help -a' and 'git help -g' lists available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.


`git add` añade archivos y cambios a una cola de commit
