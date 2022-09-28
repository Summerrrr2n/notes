Title: PDF文件批量合并
Date: 2022-9-27 18:23:53
Category: python
Tags: python, PDF

一个用于把各个文件夹中的多个pdf合并为一个pdf，并以文件夹的名字为PDF名的小脚本。

```python
import os
from PyPDF2 import PdfFileMerger

target_path = 'C:\\Users\\SummerLiu\\Downloads\\Summer'
pdf_lst = [f for f in os.listdir(target_path)]
print('pdf_lst:  ',pdf_lst)
pdf_lst = [os.path.join(target_path, filename) for filename in pdf_lst]
print('pdf_lst1:  ',pdf_lst)
for dir in pdf_lst:
    print('dir:  ',dir)
    print('os.listdir(dir):  ',os.listdir(dir))
    file_merger = PdfFileMerger()
    for pdf in os.listdir(dir):
        pdf_file = os.path.join(dir, pdf)
        file_merger.append(pdf_file)
    file_merger.write(dir+".pdf")
```