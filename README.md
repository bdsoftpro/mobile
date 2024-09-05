# Go support for Mobile devices in powershell
$env:ANDROID_HOME="D:\Sdk"
$env:ANDROID_NDK_HOME="D:\Sdk\ndk\25.1.8937393"
$env:GOPATH=($pwd).path
$env:PATH=$env:PATH+($pwd).path+"\bin;C:\Program Files\Android\Studio\jbr\bin;"
gomobile bind -target android -androidapi 23 -o calculator.aar

parameter more info:- golang.org/x/mobile/cmd/gomobile
