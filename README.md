#Description
DOL 框架描述(随着实验进行迭代添加、修改)
![](http://g.hiphotos.baidu.com/image/pic/item/8326cffc1e178a82af40ae40fe03738da877e8d6.jpg)
#How to install
####Dol 安装笔记
1. 下载文件(使用Vmware虚拟机，也可以从主机拷贝到虚拟机中)： sudo wget http://www.accellera.org/images/downloads/standards/systemc/systemc-2.3.1.tgz sudo wget http://www.tik.ee.ethz.ch/~shapes/downloads/dol_ethz.zip1
2. 解压文件 新建dol的文件夹 $ mkdir dol 将dolethz.zip解压到 dol文件夹中 $ unzip dol_ethz.zip -d dol 解压systemc $ tar -zxvf systemc-2.3.1.tgz
3. 编译systemc 解压后进入systemc-2.3.1的目录下 $ cd systemc-2.3.1 新建一个临时文件夹objdir $ mkdir objdir 进入该文件夹objdir $ cd objdir 运行configure(能根据系统的环境设置一下参数，用于编译) $ ../configure CXX=g++ --disable-async-updates 运行完之后如下图  ![](http://h.hiphotos.baidu.com/image/pic/item/c75c10385343fbf2c53477c3b87eca8065388f32.jpg)
4. 编译dol 进入刚刚dol的文件夹 $ cd ../dol 修改build_zip.xml文件 修改路径（注意，对于 64位 系统的机器，lib-linux要改成lib-linux64） 然后是编译 $ ant -f build_zip.xml all 若成功会显示build successful 接着可以试试运行第一个例子 进入build/bin/mian路径下 $ cd build/bin/main 然后运行第一个例子 $ sudo ant -f runexample.xml -Dnumber=1 成功结果如图 ![](http://f.hiphotos.baidu.com/image/pic/item/d788d43f8794a4c2985e36cb06f41bd5ac6e39d5.jpg)

#Experimental experience
简单的来说就是按照着ppt给的内容一步一步执行下去，其中遇到的问题主要是一开始直接使用国外源很难安装，后来更换成阿里云的就差不多解决了。另外的就是发现了markdown这个新大陆，感觉很强势。=。=# ES2016_14353183
# ES2016_14353183
