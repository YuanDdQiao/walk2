# walk2
来源于 lxn/walk
# 修改原因
因为无法对新版本go mod 的支持，所以修改
# 变动位置
github.com\lxn\walk\messagebox.go

    syscall.StringToUTF16Ptr(strings.ReplaceAll(message, "\x00", "␀")),
    syscall.StringToUTF16Ptr(strings.ReplaceAll(title, "\x00", "␀")),
    -->
    github.com\YuanDdQiao\walk2\messagebox.go

    syscall.StringToUTF16Ptr(strings.Replace(message, "\x00", "␀",-1)),
    syscall.StringToUTF16Ptr(strings.Replace(title, "\x00", "␀",-1)),

    "github.com/lxn/walk"
    -->
    walk "github.com/YuanDdQiao/walk2"
