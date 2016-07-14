* recall memory from 2014/09/24

# history-1

From: Jason Liang [mailto:jasonckliang@fb.com]
Sent: Wednesday, September 24, 2014 5:22 AM

Hi Joe, Kevin, Redhairer,
 
William has uploaded to quanta SFTP. Fred has done some work with this already and he can help you get started. What has been uploaded includes a) iPXE rom; b) patch to the baseline code. The baseline code we use is found here: (https://git.ipxe.org/ipxe.git/commit/f3d423b26b2baa3e4c3919c5a2e12d793043f354)


http://git.ipxe.org/ipxe.git

% elilo patch for iPXE download protocol
http://www.mail-archive.com/ipxe-devel@lists.ipxe.org/msg00856.html

# recover from /ark/zym/cook/ipxe/ipxe-fb

```
>% wget -cN "https://git.ipxe.org/ipxe.git/snapshot/f3d423b26b2baa3e4c3919c5a2e12d793043f354.tar.bz2"
mkdir 0 && cd 0
tar xf ../f3d423b26b2baa3e4c3919c5a2e12d793043f354.tar.bz2
ln -s ipxe-f3d423b a
patch -p0 < ../ipxe-fb.patch

==>

patching file a/src/config/general.h
patching file a/src/image/efi_image.c
Hunk #1 succeeded at 127 (offset 3 lines).
Hunk #2 succeeded at 155 (offset 3 lines).
Hunk #3 FAILED at 174.
Hunk #4 succeeded at 231 (offset -4 lines).
Hunk #5 succeeded at 272 (offset -15 lines).
1 out of 5 hunks FAILED -- saving rejects to file a/src/image/efi_image.c.rej
patching file a/src/include/ipxe/dhcpv6.h
patching file a/src/net/udp/dhcpv6.c
patching file b/src/setuserclass.ipxe
```



* story 1
  some thing.
```
  this is a test.
```


* story 2
  some thing.
  ```
  this is a test.
```


* story 3
  some thing.

  ```
  this is a test.
```

