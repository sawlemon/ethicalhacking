# BSidesBOS CTF

# Warmups

## Read THe Rules

https://bsidesbos.ctf.games/rules

![](2020-09-26-18-25-56.png)

![](2020-09-26-09-19-23.png)

## Kiddie Pool

kiddiepool.png 

![](ctf/kiddie_pool.png)

![](2020-09-26-09-24-15.png)

Nothing here

![](2020-09-26-09-25-45.png)
 unspiral the image by 900%

Flag Found
![](2020-09-26-09-40-43.png)




## EZ Bake Oven

Coockie in Base64 :

`echo "eyJyZWNpcGUiOiAiRG91Z2hudXRzIiwgInRpbWUiOiAiMDkvMjYvMjAyMCwgMTM6NDQ6MzgifQ==" | base64 -d `
Decoded:

{"recipe": "Doughnuts", "time": "09/26/2020, 13:44:38"}


`echo -n "{"recipe": "Magic Cookies", "time": "08/26/2020, 13:50:21"}" | base64`

eyJyZWNpcGUiOiAiTWFnaWMgQ29va2llcyIsICJ0aW1lIjogIjA4LzI2LzIwMjAsIDE0OjM0OjU3In0K

*New Cookie Value*

document.cookie="eyJyZWNpcGUiOiAiTWFnaWMgQ29va2llcyIsICJ0aW1lIjogIjA4LzI2LzIwMjAsIDE0OjM0OjU3In0K"

![](2020-09-26-10-41-24.png)

## Baseball

TzRaVUNVMlRNRTRIQTZMSFBGWkdTNVpTSzVZVU1ZSllIQk5ER00zREdKTkhBVTJWSkJHVkNWMllPRlVFSzMyRE9GTUVNMkNaR0Y1RU1VUlpNUlNHS1JSWE9CQ1VVU1pZSk4ySEFWVFVPVTJGQzJDV000WlUyUVNHSlpBVFNNUT0=

`echo "TzRaVUNVMlRNRTRIQTZMSFBGWkdTNVpTSzVZVU1ZSllIQk5ER00zREdKTkhBVTJWSkJHVkNWMllPRlVFSzMyRE9GTUVNMkNaR0Y1RU1VUlpNUlNHS1JSWE9CQ1VVU1pZSk4ySEFWVFVPVTJGQzJDV000WlUyUVNHSlpBVFNNUT0=" | base64 -d`

O4ZUCU2TME4HA6LHPFZGS5ZSK5YUMYJYHBNDGM3DGJNHAU2VJBGVCV2YOFUEK32DOFMEM2CZGF5EMURZMRSGKRRXOBCUUSZYJN2HAVTUOU2FC2CWM4ZU2QSGJZATSMQ=

`echo "O4ZUCU2TME4HA6LHPFZGS5ZSK5YUMYJYHBNDGM3DGJNHAU2VJBGVCV2YOFUEK32DOFMEM2CZGF5EMURZMRSGKRRXOBCUUSZYJN2HAVTUOU2FC2CWM4ZU2QSGJZATSMQ=" | base32 -d`

w3ASSa8pygyriw2WqFa88Z33c2ZpSUHMQWXqhEoCqXFhY1zFR9ddeF7pEJK8KtpVtu4QhVg3MBFNA92

![](2020-09-26-12-32-18.png)

Base 64 to 32 to 58 

    flag{wow_you_hit_a_homerun_and_really_ran_the_bases_there}

## Y2K

`nc challenge.ctf.games 31656`

What year do YOU think the world will end?

20000000000

Yeah! I agree with you! I also think the world will end in the year 

20000000000
 
    If a string is givcen as input

What year do YOU think the world will end?

`asdasd`

Traceback (most recent call last):
  File "/home/challenge/server.py", line 4, in <module>
    end = input()
  File "<string>", line 1, in <module>

NameError: name 'asdasd' is not defined


## Give Up

`nc challenge.ctf.games 32445`

`ls -la`
    
    total 8
    drwxr-sr-x    1 root     root          4096 Sep  4 22:43 .
    drwxr-xr-x    1 root     root          4096 Sep  4 22:43 ..

`pwd`

    /home/challenge


## Play The Harp

`exiftool harp.jpg`

    ExifTool Version Number         : 11.65
    File Name                       : harp.jpg
    Directory                       : .
    File Size                       : 280 kB
    File Modification Date/Time     : 2020:09:26 14:53:10+00:00
    File Access Date/Time           : 2020:09:26 14:53:09+00:00
    File Inode Change Date/Time     : 2020:09:26 14:53:27+00:00


`strings harp.jpg`
    
    rA<s
    N*PH
    0}{{
    p}}}{
    v?Z_
    v?Z_

---

# Forensics 

## Mercury

![](2020-09-26-11-43-22.png)

### typical file

requires

    dotencode
    fncache
    generaldelta
    revlogv1
    sparserevlog
    store

lastmessage.txt

    Y2U1ZmYzMWVhY2EyNWMwMzg1OTJhNGI3YjAxNGVjNDcK

hashid lastmessage.txt

    Unknown Hash




 ---

# Miscellaneous

## Tea Mix

`find . | grep flag 2>/dev/null`

    find . | grep flag 2>/dev/null
    find: ./root: Permission denied
    find: ./var/db/sudo: Permission denied
    ./sys/devices/pnp0/00:05/tty/ttyS2/flags
    ./sys/devices/pnp0/00:03/tty/ttyS0/flags
    ./sys/devices/pnp0/00:06/tty/ttyS3/flags


