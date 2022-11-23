# MissingSemester

# 网站

https://missing.csail.mit.edu/2020/

# Learning Notes

## Course overview + the shell

## Shell Tools and Scripting

### Finding files

history | grep XXX

```Bash
➜  ~ history | grep find   # 搜寻使用过的包含“find”的命令
 1362  grep find
 1363  history | grep find
 1364  grep find
 1365  history | grep find
 1369  find python
 1370  find fly
 1373  find qb
```

Ctrl+R

After pressing `Ctrl+R`, you can type a substring you want to match for commands in your history. As you keep pressing it, you will cycle through the matches in your history. 

一直按Ctrl+R，可以持续搜索

```Bash
➜  ~ python --version
bck-i-search: python_
```

## Editors (Vim)