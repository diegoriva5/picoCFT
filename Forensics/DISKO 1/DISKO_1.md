# DISKO 1

## Tools
- strings

# Challenge
Use the `file` command to understand what kind of image it is.

Output: 'DOS/MBR boot sector, code offset 0x58+2, OEM-ID "mkfs.fat", Media descriptor 0xf8, sectors/track 32, heads 8, sectors 102400 (volumes > 32 MB), FAT (32 bit), sectors/FAT 788, serial number 0x241a4420, unlabeled'

This means that the image contains a FAT32 filesystem, often used on USB drives.

Now we use:
`strings disko-1.dd | less` to extract all strings, and then `grep` to find the flag.

`strings disko-1.dd | grep -i picoCTF`: picoCTF{1t5_ju5t_4_5tr1n9_e3408eef}

