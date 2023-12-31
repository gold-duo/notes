
## 安装brew
 /bin/zsh -c "$(curl- fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"

## [python binding fann2](https://github.com/FutureLinkCorporation/fann2)
### python获取lib目录(`python -c "import sys; print(sys.path)"`获取)


## libFann编译
cmake -DCMAKE_INSTALL_PREFIX=/Users/obaniu.liao/SoftwareDevelop/fann-master 
cmake -DCMAKE_INSTALL_PREFIX="/usr/local/lib"


## [拷贝“libdoublefann.a"到了lib](https://pypi.org/project/fann2/)
- 1.### windows
Copy “fanndouble.lib” from FANN installed files to ${python_libs_directory} as “doublefann.lib”;

- 2.macOS
拷贝“libdoublefann.a"到了`/usr/local/lib/libdoublefann.a` 

## [使用](http://leenissen.dk/fann/html/files/fann_cpp-h.html)
```python
from fann2 import libfann
# and then create libfann.neural_net and libfann.training_data objects
ann = libfann.neural_net()
train_data = libfann.training_data()
# Look at the examples in the FANN documentation and its C++ bindings for further reference.
```

## 其他
cmake -DCMAKE_INSTALL_PREFIX="/System/Library/Frameworks/Python.framework/Versions/2.7/lib/"
https://blog.csdn.net/sinat_35576477/article/details/120573664

- [python pypi 地址](https://pypi.org/project/fann2/)

