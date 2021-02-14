
# Listing files and directories

## Make many random files 
** seq -w 1 10 | xargs -n1 -I% sh -c 'dd if=/dev/urandom of=file% bs=$(shuf -i1-10 -n1) count=1024' **
```
file01  file02  file03  file04  file05  file06  file07  file08  file09  file10
```

