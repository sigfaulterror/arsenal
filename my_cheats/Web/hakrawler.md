# Hakrawler
#plateform/linux #target/remote #cat/RECON #tag/http

## Hakrawler - crawle single target

Fast golang web crawler for gathering URLs and JavaScript file locations. This is basically a simple implementation of the awesome Gocolly library.

https://github.com/hakluke/hakrawler
```
echo <target> | hakrawler -u -insecure -w -json |tee <out_file>
```

## Hakrawler - crawle multiple targets

Fast golang web crawler for gathering URLs and JavaScript file locations. This is basically a simple implementation of the awesome Gocolly library.

https://github.com/hakluke/hakrawler
```
cat <targets_file> | hakrawler -u -insecure -w -json |tee <out_file>
```