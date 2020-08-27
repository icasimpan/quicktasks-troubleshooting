---
title: "Zip a Text File using 256-AES Encryption"
date: 2020-08-28T00:20:25+08:00
tags: [troubleshooting, zip, encryption, aes]
draft: false
---

Use the following command:
```
7z a -p -mem=AES256 -tzip file.zip source-file1.txt source-file2.txt
```

It will ask for a password but will obviously not be echoed.

To decrypt:
```
7za e file.zip
```

Some details https://unix.stackexchange.com/questions/182573/how-strong-is-the-encryption-of-a-zip-file-in-linux-mint
