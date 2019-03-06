# Ipynb_importer 在Jupyter notebook 中引用其他ipynb文件

Reference:
https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Importing%20Notebooks.html  

# How to use it
For jupyter notebook. create a file with the provided codes, put it in the same folder where you work. 
Then, import this file like a module, then you can import other ipynb files in the same way as importing modules.   

import Ipynb_importer  
import the_file_you_need as you_like  

Then, you have access to the methods and variables in the_file_you need

# Problem so far
It works for my first folder. However, when I tried for another folder, it failed. 

# Solutions:
Append the path of the folder where the first Ipynb_importer that worked is to your current path. 
Then, you can import other files. 

# 使用：
1. 在当前文件夹，创建一个新文件，命名为Ipynb_importer或者你随便给的什么名字。
2. 拷贝代码
3. 在当前文件，import Ipynb_importer， 再import其他你需要的文件。

# 遇到的问题：
第一次尝试，在第一个文件夹成功了。后来在另一个文件夹里，总是显示Ipynb_import undefined。

# 解决：
在当前工作路径下，用sys.append(),把之前运行没问题的Ipynb_importer所在的文件夹路径加上。然后就可以import了。 
