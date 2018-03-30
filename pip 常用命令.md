# pip常用命令
[转自](http://me.iblogc.com/2015/01/01/pip%E5%B8%B8%E7%94%A8%E5%91%BD%E4%BB%A4/)
---
### 1. 已安装的包

```
pip freeze or pip list
```
### 2. 导出requirements.txt

```
pip freeze > <目录>/requirements.txt


```
### 3.在线安装

```
pip install <包名> 或 pip install -r requirements.txt


```
### 4.安装本地安装包

```
pip install <目录>/<文件名> 或 pip install --use-wheel --no-index --find-links=wheelhouse/ <包名>

<包名>前有空格

可简写为

pip install --no-index -f=<目录>/ <包名>

```
### 5.卸载包

```
pip uninstall <包名> 或 pip uninstall -r requirements.txt


```
### 6.升级包

```
pip install -U <包名>


```
### 7.升级pip

```
pip install -U pip


```
### 8.显示包所在的目录

```
pip show -f <包名>


```
### 9.搜索包

```
pip search <搜索关键字>


```
### 10.查询可升级的包

```
pip list -o


```
### 11.下载包而不安装

```
pip install <包名> -d <目录> 或 pip install -d <目录> -r requirements.txt


```
### 12.打包

```
pip wheel <包名>


```
### 13.国内pypi镜像
- 豆瓣：https://pypi.douban.com/simple
- 中国科学技术大学：https://mirrors.ustc.edu.cn/pypi/web/simple/
- 清华大学TUNA：https://pypi.tuna.tsinghua.edu.cn/simple
https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/