# How To Decompile Android Apk

- REQUIRED (on Mac OSX)

1. dex2jar-2.0
http://sourceforge.net/projects/dex2jar/?source=typ_redirect
2. apktool_2.0.1.jar
https://bitbucket.org/iBotPeaches/apktool/downloads
3. jd-gui
http://jd.benow.ca

- How to install apktool(on Mac OSX)  
http://ibotpeaches.github.io/Apktool/install  
1. Download Mac wrapper script (Right click, Save Link As apktool)  
2. Download apktool-2 (find newest here)  
3. Rename downloaded jar to apktool.jar  
4. Move both files (apktool.jar & apktool) to /usr/local/bin (root needed)  
5. Make sure both files are executable (chmod + x)  
6. Try running "apktool" command via cli  

- How to use dex2jar-2.0

first, you should do:  
chmod 777 *.sh

# 1ST PART(*.java source code)

1. download source tmp.apk from:  
http://www.wandoujia.com/
  
- USING dex2jar-2.0
  
1. cd dex2jar-2.0/  
2. ./d2j-dex2jar.sh ../tmp.apk  
3. RESULT:  
../tmp.apk -> ./tmp-dex2jar.jar 
  
- USING jd-gui  

1. drags tmp-dex2jar.jar into jd-gui  
2. save all sources  
3. get *.java  

# 2ND PART(XML source code)  
  
- USING apktool  
  
1. apktool d tmp.apk  
2. generates a folder called tmp  