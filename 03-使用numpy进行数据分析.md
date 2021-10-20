# Numpy数据分析

#### 读写文件

> ==save==函数==>以**二进制**的格式保存数据(单个).npy

```python
np.save(file,arr,allow_pickle=True,fix_imports=True)
#file	保存文件的名称，未设置则为默认目录
#arr	需要保存的数组
#把数组arr保存到名称为'file'的文件中，文件扩展名为.npy系统自动添加
```

> ==savez==函数==>和save一样(多个).npz

```python
np.savez('……',arr1,arr2)
#把数组arr1与arr2一同保存到名称为……的文件中，文件扩展名为.npz系统自动添加
```

> ==load==函数==>读取二进制文件(文件名需要加后缀)

```python
np.load('…….npy')		#读取含有单个数组的文件
loaded_data=np.load(r'…….npz')		#读取文件的全部数组
loaded_data['数组名']		#读取文件中的某一数组
```

> ==savetxt==函数==>将数组写道以某种分隔符隔开的文本文件中

```python
np.savetxt(fname,X,fmt='%d',delimiter=' ',newline='\n',header='',footer='',comments='#')
#fname	文件名
#X	数组数据
#delimiter=''(分隔符,默认为空格)
#fmt=''(保存格式，%d整型)
```

> ==loadtxt==函数

 























