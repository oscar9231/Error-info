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
