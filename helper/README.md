gin-slim-helper
===============
Utility helper for Gin framework

## Usage

```Go
// Md5
m := helper.Md5("123")
log.Println(m)

// Random string
r := helper.RandStr(12)
log.Println(r)

type T struct {
    A string
    B int
}

// Json2String
s := T{"a", 123}
ss := helper.Json2String(s)
log.Println(ss)

// String2Json
sss := new(T)
helper.String2Json(ss, sss)
log.Println(sss)

// Check file exist
e := helper.FileExists("./main.go")
log.Println(e)

// Check is dir
id := helper.FileIsDir("./main.go")
log.Println(id)