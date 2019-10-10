# redhat 安装 rlwrap
-------------------------

> rlwrap工具可以为dbaccess提供浏览历史命令行的功能,和删除先前输入错误的字母等问题。有了这个工具informix的dbaccess就可以顺利的执行上下箭头的功能。

### 首先需要安装readline
> yum install readline-devel 

### 源码安装 rlwrap
> tar zxvf rlwrap-*.tar.gz  
> ./configure  
> make  
> make install

### 设置 dbaccess 别名
> alias dbaccess='rlwrap dbaccess'
