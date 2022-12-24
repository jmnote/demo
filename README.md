# demo

```
git clone https://github.com/jmnote/demo.git
cd demo
javac -d bin -cp "lib/*" src/*
java -cp "bin;lib/*" App
```

Windows (OK)
```
PS C:\Users\user01> git clone https://github.com/jmnote/demo.git
Cloning into 'demo'...
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (7/7), done.
remote: Total 10 (delta 1), reused 6 (delta 0), pack-reused 0
Receiving objects: 100% (10/10), 249.38 KiB | 22.67 MiB/s, done.
Resolving deltas: 100% (1/1), done.

PS C:\Users\user01> cd demo
PS C:\Users\user01\demo> javac -d bin -cp "lib/*" src/*
PS C:\Users\user01\demo> java -cp "bin;lib/*" App
hello
{serializeNulls:false,factories:[Factory...
```

Linux (Error)
```
root@linux01:~# git clone https://github.com/jmnote/demo.git
Cloning into 'demo'...
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (7/7), done.
remote: Total 10 (delta 1), reused 6 (delta 0), pack-reused 0
Unpacking objects: 100% (10/10), done.

root@linux01:~# cd demo
root@linux01:~/demo# javac -d bin -cp "lib/*" src/*
root@linux01:~/demo# java -cp "bin;lib/*" App
Error: Could not find or load main class App
Caused by: java.lang.ClassNotFoundException: App
```

