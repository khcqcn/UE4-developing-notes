# UE4 项目资源打包,Pak包生成过程

* 项目打包过程:

1 工具代码编译

2 项目,引擎代码编译

3 资源COOK(烘培)

4 文件整理收集

5 资源打包

6 文件拷贝(exe,dll文件拷贝)

 

* Pak包生成是通过UnrealPak.exe来完成的

通过运行时传递参数 UnrealPak.exe [要生成的pak文件] -create=[要打包的文件列表] -order=[文件在pak中排序描述文件] [输出格式] [是否加密] [是否压缩]

> UnrealPak.exe test.pak -create=paklist.txt -order=CookerOpenOrder.log -UTF8Output -encrypt -compress
