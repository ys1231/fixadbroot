# fixadbroot
修复安装`magisk`之后 `adb root` 会报错
`adbd cannot run as root in production builds`

**如果安装了shamiko 需使用修改版 做了两件事**
1. 修改 service.sh 中 check_reset_prop "ro.debuggable" "1" 
2. 修复 service.sh.sha256 sha256

Shamiko-v0.6-126-debug 对应 magisk v25

Shamiko-v0.7-161-debug 对应 magisk v26

# 注意 修改Shamiko破坏了完整性so里面应该做了校验,所以需要关闭Shamiko才可以生效.
[参考链接](https://liwugang.github.io/2021/07/11/magisk_enable_adbr_root.html) 分析的很详细值得学习.

