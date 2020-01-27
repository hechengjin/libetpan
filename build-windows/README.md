## libEtPan on Windows ##

All the provided binaries are compiled in release mode.
For the debug mode, you need to download the repositories and compile them.

### Binary ###

In case you just need a binary build of libEtPan:
- [libEtPan](http://d.etpan.org/mailcore2-deps/libetpan-win32/)

Also, you'll need all the dependencies, download the most recent binary builds in:

- [Cyrus SASL](http://d.etpan.org/mailcore2-deps/cyrus-sasl-win32/)
- [zlib](http://d.etpan.org/mailcore2-deps/zlib-win32/)
- [OpenSSL](http://d.etpan.org/mailcore2-deps/misc-win32/)
- [SASL](http://d.etpan.org/mailcore2-deps/cyrus-sasl-win32/)

### Build using Visual Studio 2013 ###

You'll need all the dependencies, download the most recent binary builds in:

- [zlib](http://d.etpan.org/mailcore2-deps/zlib-win32/)
- [OpenSSL](http://d.etpan.org/mailcore2-deps/misc-win32/)
- [SASL](http://d.etpan.org/mailcore2-deps/cyrus-sasl-win32/)

#### Instructions for zlib ####

- copy `include`, `lib` and `lib64` folders to `libetpan/third-party`.

#### openssl ####

- copy `bin`, `bin64`, `include`, `lib` and `lib64` to `mailcore2/Externals`.

As a result, in `Externals` folder, you should have the following folders: `include`, `lib`, `lib64`, `bin` and `bin64`.

In `libetpan/build-windows`, using Visual Studio 2013, open `libetpan.sln`.
Then, build.

Public headers will be located in `libetpan/build-windows/include`.

相关依赖包下载：
链接：https://pan.baidu.com/s/1pMwcPZH
 密码：0jro
 
 
 测试程序使用方法
 readmsg.exe -d imap -s imap.139.com -p 143 -u xx@139.com -v password -l INBOX 2445 2446 
 
 smtpsend.exe -f firemail_wang@126.com -u firemail_wang@126.com -v password -s smtp.126.com -p 25 rec1@163.com rec2@189.cn  ------------回车后，再一起输入如下绿色内容
Date: Fri, 08 Dec 2017 10:28:32 +0800
To: 15313159857@163.com
From: firemail_wang@126.com
Subject: test Fri, 08 Dec 2017 10:28:32 +0800
Message-Id: <20171208102831.010808@qq.com>
X-Mailer: swaks v20170101.0 jetmore.org/john/code/swaks/


This is a test mailing                                   ----------- 回车后按Ctrl+Z再回车
^Z
Sent ok.                      
