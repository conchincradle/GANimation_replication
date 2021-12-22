https://www.cosineg.com/archives/11/

#OpenFace入门心得

直接使用

在https://github.com/TadasBaltrusaitis/OpenFace/releases处直接下载编译好的文件，解压。但是还不能运行，要额外下载模型（通过OneDrive）：

scale 0.25

scale 0.35

scale 0.50

scale 1.00

四个模型文件全部下载完后，放入OpenFace文件夹下 model\patch_experts内。

文件夹下有数个可执行文件，这里挑三个常用的。

FaceLandmarkImg.exe

这个程序用来处理照片。在当前目录下打开控制台（CMD或powershell），运行

.\FaceLandmarkImg.exe -f .\samples\sample1.jpg

其中 -f 参数代表处理单个文件，后接文件路径，-fdir 参数则是处理文件夹。

等程序运行完毕后，会在目录下生成processed文件夹，里面包含有处理完（加上特征点与注视方向等内容）的照片和保存了处理数据（特征点坐标、AU强度等）的csv文件等。

******************************************我的*******************************************

##download in to files in computer，download four scale files into model\patch_experts

##put images you want to process into samples\imgs

##open powershell on current directory

##run .\FaceLandmarkImg.exe -fdir .\samples\imgs -aus    (aus is for GANimation, we only need AU vectors)

##then the csv files will be output in processed file

##put the csv files in files in GANimation program for next step to output an aus_openface.pkl file

