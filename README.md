gc
==

auto read task from todo file &amp;&amp; commit ; then delete the finish task
e.g.
### todo file
    task a
    xxxxx

    task b
    xckfl

    task c
    xxxdfkl

    task d
    fkdlflf

### ./gc (may be, you would like add it to your PATH, so you can simple run gc)

    # On branch master
    # Changes to be committed:
    #   (use "git reset HEAD <file>..." to unstage)
    #
    #   modified:   server.js
    #
    # Untracked files:
    #   (use "git add <file>..." to include in what will be committed)
    #
    #   .gc.swp
    #   gc
    #   node_modules/
    #   todo
    #   todo2
    #   todon
    任务描述：
         task b
         xckfl

     如果不要提交请选择(n|N), 其他任意键则提交:

### then touch enter on the keyboard and you will get:
    [master 9e6b67f] task b xckfl
     1 file changed, 1 insertion(+), 3 deletions(-)
     ok, 接下来的任务是：
         task c
         xxxdfkl


### don't forget add todo file to your .gitignore file !!!
