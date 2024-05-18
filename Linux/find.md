# Find

Search for files in a directory hierarchy

> find [path] [options]

## options

###  -name

-  `-name [filename]`

```sh
┌──(kali㉿kali)-[~/find]
└─$ find . -name '*.txt' 
./a.txt
./b.txt
```

### -type

- `-type f` : only file
- `-type d` : only folder

```sh
┌──(kali㉿kali)-[~/find]
└─$ find ./ -type f -name 'a' 
./a
```

### -exec

execute a command every item in the results

- `-exec [command] {} +`
    - `{}` : item itself
    - `+` : end of command

```sh
┌──(kali㉿kali)-[~/find]
└─$ find . -type f -exec chmod 600 {} +
```

---

*https://youtu.be/skTiK_6DdqU*
