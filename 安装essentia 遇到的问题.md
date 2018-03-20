# 在此处输入标题

标签（空格分隔）： 未分类

---

在此输入正文

essentia 音频软件包遇到的问题！

主要是安装下面两个链接来安装essentia 音频软件包
https://github.com/MTG/essentia/tree/master

http://blog.csdn.net/chen0ming123/article/details/50930086

在安装Essentia的过程中出现一个问题:
安装官网的步骤操作的下面的步骤:
./waf configure --mode=release --build-static --with-python --with-cpptests --with-examples --with-vamp --with-gai

./waf

会出现：
Build failed
 -> task in 'essentia_standard_onsetrate' failed with exit status 1 (run with -v to display more information)
 -> task in 'essentia_standard_mfcc' failed with exit status 1 (run with -v to display more information)
 -> task in 'essentia_standard_beatsmarker' failed with exit status 1 (run with -v to display more information)
 这样的错误。
 最后解决的方法是：
 ./waf configure --build-static --with-python --with-cpptests --with-examples --with-vamp
 参考链接：https://github.com/MTG/essentia/issues/558
 