## LipsonX Gogs Version
The Gogs project is dead; I maintain this version personally mainly to address security issues and other problems. It's a personal version. Not recommended for use.

feature:
- Pure go sqlite
- Patch [Snoar CVE-2024 Solution](https://www.sonarsource.com/blog/securing-developer-tools-unpatched-code-vulnerabilities-in-gogs-1/)


## build
```
go get github.com/glebarez/sqlite
go get modernc.org/sqlite
go get  xorm.io/core
go get  xorm.io/build
go get  xorm.io/xorm

GOOS=linux CGO_ENABLED=0 GOARM=5 GOARCH=arm go build
```
