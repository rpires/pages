- [ ] download latest S image and create the AVD
[one](emul1.png) [two](emul2.png)
**if the avd will start, but the adb will always return:  'device not connected':**
- [ ] delete the avd
- [ ] donwload S02 image https://dl.google.com/android/repository/sys-img/google_apis/arm64-v8a-S_r02.zip
- [ ] replace in folder
```shell
cd ~/Library/Android/sdk/system-images/android-S/google_apis_playstore
copy -r ~/Downloads/arm64-v8a .

```
- [ ] re create the avd in android studio
- [ ] verify the emultor is working by running adb
```shell
# runing
adb devices
# should show
List of devices attached
emulator-5554	device
```