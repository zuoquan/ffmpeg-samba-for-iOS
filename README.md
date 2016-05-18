# ffmpeg-samba-for-iOS
iOS端ffmpeg支持samba协议的播放，编译ffmpeg前需要先编译samba库（samba的编译脚本位于samba--文件夹下的rakefile执行rake即可）
当前编译的是arm64指令集 若需要支持其他指令集修改rakefile最后编译选项即可!

ffmpeg的编译需要根据samba库的位置去配置--extra-cflags和--extra-ldflags选项若要支持samba则需要打开--enable-libsmbclient
详细见build_ffmpeg_arm64脚本。
