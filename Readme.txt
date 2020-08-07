2020-8-6
        克隆自https://sourceforge.net/p/stm32flash/code/ci/master/tree/
编译方法
        在linux下：make即可，如需安装则sudo make install
        在window下：
        1.到“http://www.cygwin.com/”下载setup-x86_64.exe并默认安装。默认安装是没有gcc和make的
        2.在安装文件的目录打开命令行，并输入：
        setup-x86_64.exe -q -P wget -P gcc-g++ -P make -P diffutils -P libmpfr-devel -P libgmp-devel -P libmpc-devel  
        3.出现note: Hand installation over to elevated child process.表明安装完成
        4.双击Cygwin64 Terminal定位到源代码目录，make即可
2020-8-7
        上面第3条描述有误。第二种方式是运行setup-x86_64.exe到Select Packages页，选择View中的Full再在列表中选择需要的包
        使用cygwin编译会依赖于cygwin1.dll，需要把cygwin安装目录下的cygwin1.dll复制到应用程序目录或C:\Windows\System32