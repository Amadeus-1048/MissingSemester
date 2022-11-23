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

### Modal Editing

- Vim has multiple operating modes.

  - **Normal**: for moving around a file and making edits

  - **Insert**: for inserting text     ( Normal to Insert : i)

  - **Replace**: for replacing text

  - **Visual** (plain, line, or block): for selecting blocks of text   ( Normal to Visual : v)

  - **Command-line**: for running a command

  Vim 五种模式：

  - 普通模式：执行 Vim 的指令，如移动光标，复制 / 删除 / 粘贴文本等等，不能打字输入。

  - 插入模式：进行文本输入（打字）, 和普通编辑器一样

  - 替换模式：进行字符替换

  - 可视模式：进行文本选择

  - 命令模式：在 Vim 底部最后一行中输入命令，按回车并执行



### Visual mode

Normal 模式下，命令的语法可以总结为 verb + noun, 比如 dG 命令，d 是动词，表示删除，G 表示最后一行，所以是删除到最后一行。而在 visual mode 下，由于我们已经选中了区域，这就是 noun, 所以只需要再提供 verb 即可。 但是此时的行为会有些不同，举几个例子来说明

- x: Normal mode 下是删除一个字符，Visual mode 下是删除整个选中区域

- r: Normal mode 下是用接下来输入的单个字符来代替当前字符，而Visual mode 下会复制多次该字符，保证行的长度不变