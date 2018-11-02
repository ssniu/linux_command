which


find
  -name:
  -perm:
  -prune: 
  -user:
  -group:
  -mtime: -n, +n, n
  -nogroup:
  -nouser:
  -newer file1 ! file2: 查找比file1新但比file2旧的文件
  -size:
  -depth: 
  
  类型
  -b: block 
  -d: directory
  -c: character 
  -p: pipeline
  -l: symbolic file
  -f: regular file
  
  操作
  -print:
  -exec:
  -ok:
  
  examples:
  $find . -name "t*" -perm 744 -print
  $find . -mtime -90 -print
  $find /etc -type f -name "rc*" -exec ls -l { } \;
  $find /etc -type f -ok rm {} \;
  

locate


which


whereis
