#vimtutor


### Vim Commonds

```bash

    ================================================================

    <ESC>               // 进入正常模式
    a                   // 进入插入模式
    v                   // 进入可视模式
    
    === 移动光标 ====================================================
    
    // motion
    h                   // 左移一位
    j                   // 下移一位
    k                   // 上移一位
    l                   // 右移一位

    w                   // 从当前位置移动到下一个单词的起始处，不包括它的第一个字符
    e                   // 从当前位置移动到单词的末尾，包括最后一个字符
    $                   // 从当前位置移动到行末
    2w                  // 向前移动两个单词（数字可变）
    3e                  // 向前移动至第三个单词尾（数字可变）
    0                   // 移动至行首

    === VIM的进入和退出 =============================================
    
    <ESC> + :q!         // 退出：强制，不保留修改内容

    === 文本编辑 ====================================================

    vim FILENAME
    x                   // 删除
    i                   // 插入
    A                   // 添加

    d2w                 // 删除：operator + number + motion 可以组合操作
    2dd                 // 删除：dd -> 删除整行 | 2dd -> 删除两行
    
    u/U                 // 回退：u -> 回退一步；U -> 回退整行修改
    CTRL+R              // 前进
    
    y                   // 复制：可以和v键结合复制
    p                   // 粘贴：将最后一次删除的内容置入光标之后
    
    r*                  // 替换：*为想替换的字符，可以替换光标所在的内容
    R*                  // 替换：同上，可连续替换多个字符
    ce                  // 更改：更改文本直到一个单词的末尾，ce不仅仅删除了一个单词，还进入了插入模式
    c2e                 // 更改：operator + number + motion 可以组合操作

    G                   // 跳转：跳转至文本最后一行
    gg                  // 跳转：跳转至文本第一行
    CTRL+G              // 显示当前文本的状态信息

    v                   // 选中：按下v键使vim进入可视模式，可以对文本进行高亮选择
    o/O                   // 插入：将在光标下(o)/上(O)开新的一行，同时进入插入模式
    
    === 外部命令 ===================================================

    %                   // 查找：查找配对的'(' , '[', '{'
    :s/aaa/bbb          // 将该行匹配到的第一个aaa替换成bbb
    :s/aaa/bbb/g        // 将该行匹配到的所有aaa替换成bbb
    :#,#s/aaa/bbb/g     // 将两行内匹配到的所有aaa替换成bbb
    :%s/aaa/bbb/g       // 将全文内匹配到的所有aaa替换成bbb
    :%s/aaa/bbb/gc      // 将全文内匹配到的所有aaa替换成bbb，并逐个询问操作者

    :!l*                // 在正常模式下输入:!*(* -> 一个外部命令)，可以执行外部命令
    :!ls                // 查看当前文件目录
    :!rm FILENAME       // 删除指定文件(FILENAME)

    :r FILENAME         // 提取和合并文件 ？？（第五讲第四节）不是很熟

    :set hlsearch       // 高亮显示被搜索部分

    ================================================================
    
    ??: 第四讲第二节 || 第六讲第五节

```


### Linux Commonds

```bash

    mkdir 文件夹


```