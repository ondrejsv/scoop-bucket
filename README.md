# Setup Scoop

```
Set-ExecutionPolicy RemoteSigned -s cu -force
iex (new-object net.webclient).downloadstring('https://get.scoop.sh')
scoop install git
scoop bucket known | % { scoop bucket add $_ }
scoop update
```

# Add this bucket
```
scoop bucket add ondrejsv https://github.com/ondrejsv/scoop-bucket
```