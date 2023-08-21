

## Qt对话框问号移除

```python
dialog.setWindowFlags(Qt.WindowCloseButtonHint)
```

## list_view透明背景

```python
list_view.setStyleSheet('background-color: rgba(20, 32, 255, 0);')
```



## pyinstaller打包


- 常用
  - -F 打包成一个文件（。exe文件）
  - -D 打包成多个文件 （产生一个目录(包含多个文件)作为可执行文件）
  - -w 不显示控制台
- -n 文件名
  - -i图标文件

- -C 使用控制台，无窗口


```bash
C:\Python39\Scripts\pyinstaller.exe -D -w xp_launch.py
```

## Maya2022-python2模式

```bash
set MAYA_PYTHON_VERSION=2
```



## 设置字体

```python

font = xm.font()

font.setPointSize(13)
font.setFamily('方正舒体')
#font.family()

xm.setFont(font)

for w in xm.findChildren(QtWidgets.QWidget):
    w.setFont(font)

# 获取可用字体
database = QtGui.QFontDatabase()
for x in database.families():
    print x

```







