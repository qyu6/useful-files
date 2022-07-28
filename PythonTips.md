#### (2022.7.28更新)
(Python Coding笔记)

1.一键打开经常用的多个网页
```import webbrowser
websites = [
    'www.google.com',
    'www.bing.com',
    'www.yahoo.com'
]
for url in websites:
    webbrowser.open(url)
    ```

2.在服务器中定位当前绝对路径
```
import os
current_path = os.path.abspath('<file.name.xxx>')
print(current_path)
```

3.pip批量安装依赖第三方库
```
create 'requirement.txt' file
file format like 'pandas==0.1.1'
then run 'pip install -r requirements.txt' in terminal
```