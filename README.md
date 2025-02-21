# how to run an emurator with docker 
for me i find it dificlut to enable virtualization on bios so i start an enumartor using docker 

```sh
docker run --rm -d --privileged -p 6080:6080 -p 5555:5555 -e DEVICE="Samsung Galaxy S10" budtmo/docker-android:emulator_11.0
```
- after running you should connect yoru emurator to the adb using the following command 

```sh
adb connect localhost:5555
adb devices  # Check if it's listed
```
- run expo app using 
```sh
npx expo start
```
- press `a` to open on andorid emulator 
