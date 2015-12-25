If you are using Ubuntu or a similar Linux distribution and video playback doesn't work or crashes when you start then it is likely caused by a faulty plugin cache. To refresh the cache, type the following at the shell:
```
$ sudo /usr/lib/vlc/vlc-cache-gen -f /usr/lib/vlc/plugins/
```