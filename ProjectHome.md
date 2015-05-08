在Android上的ffmpeg的剪裁和移植，包含ffmpeg源文件、JNIMakefile、类包裹文件等，只需要将jni目录放入自己工程，以及放入在源文件中放入FFmpeg.java，就可以实现FFmpeg的解码了。


压缩文件包括：jni文件夹、生成的库、以及调用类

使用方法：1 按照http://blog.csdn.net/cazicaquw/article/details/8426475
生成一个ffmpeg库，得到libffmpeg.so，放入ndk的编译目录
2 编译jni文件夹，得到libmyffmpeg.so,压缩包内包含了该库
3 将调用类文件放入源代码中