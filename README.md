# fcitx-pinyin-thesaurus-custom
Add sougou pinyin thesaurus in fcitx's thesaurus.
## How to use?
Download these two `.mb` files, copy them to `/usr/share/fcitx/pinyin` and restart fcitx.
## How to create my own thesaurus?
Use this thing:[scel4mb](https://github.com/zhanghua000/scel4mb), download a sougou pinyin thesaurus， enter the scel4mb directory, execute `./sgscel2fcitx YourThesaurusPath`, then, execute `cat sg_pyPhrase.org >> pyPhrase.org` and `./noOverlap`, the latter command may take too much time, don't worry, just wait until it finishes. At last, there will be a new file named `tmp.txt`, remove `sg_pyPhrase.org` and `pyPhrase.org`, rename `tmp.txt` to `pyPhrase.org`, if you have more thesauruses, do those things again until you add everything into `pyPhrase.org`,finally, execute `./createPYMB gbkpy.org pyPhrase.org` you wil get two files with the same names in this repository.
## Note: 
you may need `libXft.so.2` ,it is provided by `lib32-libxft` in Arch Linux, other distributions may have similar name.
Add these sougou pinyin thesauruses in these files:
![.scel file list](https://github.com/zhanghua000/fcitx-pinyin-thesaurus-custom/raw/master/Screenshot_20200316_120636.png)

## 中文
### 怎样使用？
下载这个仓库里面的`.mb`文件，复制到`/usr/share/fcitx/pinyin`然后重启fcitx就可以了
### 怎样创建自定义的词库？
使用这个工具：[scel4mb](https://github.com/zhanghua000/scel4mb)，下载搜狗拼音的细胞词库，进入这个工具的目录，执行`./sgscel2fcitx 细胞词库位置`，之后执行`cat sg_pyPhrase.org >> pyPhrase.org` 和 `./noOverlap` ,后面一个指令会要很长时间，等它处理完，之后移除`sg_pyPhrase.org`和`pyPhrase.org`，把新生成的`tmp.txt`重命名为`pyPhrase.org`，如果还有其他的词库，重复以上操作直到一切都弄好了，最后执行 `./createPYMB gpgkey.org pyPhrase.org` 这会得到类似的两个`.mb`文件。
### 注意：
缺少`libXft.so.2`时在Arch Linux下安装`lib32-libxft`，其他Linux发行版请自行查找相似软件包。
这个项目的文件加入了以下搜狗拼音细胞词库：
![细胞词库列表](https://github.com/zhanghua000/fcitx-pinyin-thesaurus-custom/raw/master/Screenshot_20200316_120636.png)
