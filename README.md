# RandomWallpaper

## Instruction in English 
1、git clone or download and extra the file to a directory where it won't bother you 

2 、Inside a terminal, cd into the BestDailyWaper-master folder, then run 
sudo sh ./install like:
```
xxx@xxx:~/BestDailyWallpaper$ sudo sh ./install
```

3、find the wallpaper from System Setting->Appearance

## 中文安装手册
1、git clone或者下载zip包并解压到任意路径。

2、在终端进入BestDailyWallpaper-master目录，并输入 sudo sh ./install 即可完成安装

3、在system setting ->Appearance 找到背景

## 修复之前BestWallpaper duration bug
之前BestDailyWallpaper设置2小时间背景在转变状态<transition>，但是因为两幅图片场景相同仅色差不同所以看不出来，但对于一天中如果时不同场景的图片则会看到两个图片处于叠加状态。

## 删除之前BestWallpaper /usr/share/gnome-background-properties/下xml文件多余路径

仅须告诉xml位置即可。
如果告诉图片位置则可以增加固定的背景图片，这里将其删除。

```
<wallpapers>
  <wallpaper deleted="false">
    <name>Daily Wallpapers</name>
    <filename>/usr/share/backgrounds/Randomwallpaper/BestRandomWallpaper.xml</filename>
    <options>zoom</options>
  </wallpaper>
```
