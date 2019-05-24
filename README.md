# StepCountVersion
运动管理系统版本配置



​	为实现软件自动更新功能，将APK文件和更新的json配置文件放置github。每次Android点击软件更新时，读取github的配置文件，然后与本地的APK版本进行比较，当本地版本较低时，则出现弹出框提示下载。用户可以选择是否下载以及后续安装步骤。



​	配置文件中有APK地址，安卓端根据该地址执行下载任务。

​	所以当软件出现新版本之后，将新版本APK上传到github本仓库中，然后修改对应配置文件中的
版本号和更新日志即可！



配置文件说明：

```json
{
  "url":"https://github.com/Mindyu/StepCountVersion/blob/master/app-release.apk?raw=true",
  "versionCode":2,
  "updateMessage":"1. 适配 Android 8.0\n2. 适配 Android 9.0\n3. 更新说明"
}
```

> url：APK下载地址
>
> versionCode：版本号
>
> updateMessage：更新日志说明