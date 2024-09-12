basename
Examples:
  basename /usr/bin/sort          -> "sort"
  basename include/stdio.h .h     -> "stdio"
  basename -s .h include/stdio.h  -> "stdio"
  basename -a any/str1 any/str2   -> "str1" followed by "str2"

```
echo "name,age,location" | cut -d',' -f2
# Output: age
```
e.g.
```
  environment="$(basename "$artifact" | cut -d'_' -f1)"
  region="$(basename "$artifact" | cut -d'_' -f2 | cut -f 1 -d '.')"
```