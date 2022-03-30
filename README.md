# GPU server

error:
```
pip install package, no permission
```
solution:
```
pip install --user package, to install on home directory
```

# librosa

error:
```
pyin function generates nan in f0
```
solution:
```
改用yin function，因为pyin会对unvoiced部分pad nan
```

error:
```
Could not find a `llvm-config` binary
```
solution:
```
pip install --upgrade pip 升级pip
```


# decomposition.PCA

error:
```
Input contains NaN, infinity or a value too large for dtype('float64')
```
solution:
```
1. 检查序列中是否有NaN值: print(np.isnan(spt_A).any())
2. 多半由于对0进行了处理, 所以想办法去掉0
```

# Biosppy

error:
```
ufunc 'multiply' did not contain a loop with signature matching types (dtype('<U12'), dtype('<U12')) -> dtype('<U12')
```
solution:
```
U32是长度为32个字节的无符号整数类型，需要转换为float格式
```

# Wav2vec

# MSE Loss

error:
```
loss or tensor为nan
```
solution:
```
normalization的时候给std加一个非常小的余项。比如：std + 0.01，避免数据中出现0，导致除以0出现nan
```

# Matplot

error:
```
不显示图像
```
solution:
```
更换后端：
import matplotlib
matplotlib.use('TkAgg')
import matplotlib.pyplot as plt
```
error:
```
plt.show()报错：
Process finished with exit code 139 (interrupted by signal 11: SIGSEGV)
```
solution:
```
升级matplot
```
