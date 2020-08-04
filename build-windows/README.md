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

### Build using Visual Studio ###

1. You need a working installation of Visual Studio 2013, 2015 or 2017. A community
edition is enough.

2. Clone repository/or download the a .zip and unpack it. The direcory where
the content of the repository lays in will from now on referenced as `libetpan`.
This `README.md` should be at `libetpan/build-windows/README.md`.

3. You'll need all the dependencies, download the most recent binary builds in:

- [zlib](http://d.etpan.org/mailcore2-deps/zlib-win32/)
- [OpenSSL](http://d.etpan.org/mailcore2-deps/misc-win32/)
- [SASL](http://d.etpan.org/mailcore2-deps/cyrus-sasl-win32/)

4. Create the `libetpan/third-party` folder.

5. Inside all the downloaded archives you should find `bin`, `bin64`, `include`,
`lib`, `lib64` or `ssl` folders. Copy all of them to `libetpan/third-party`. If you're unsure just copy
all of those folders to `libetpan/third-party`.

6. As a result, in `libetpan/third-party` folder, you should have the following folders:
- `include`
- `lib`
- `lib64`
- `bin`
- `bin64`
- `ssl`

7. In `libetpan/build-windows`, using Visual Studio, open `libetpan.sln`.

8. Build the solution


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
