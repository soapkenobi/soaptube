# SoapTube
Requires:
- Zulu JDK 17
- x64 OS
- Supported Youtube apk(Current=17.29.34); make sure apk is not bundle

To run execute:

```bat
java -jar builder.jar -b patches.jar -m integrations.apk -a youtube.apk -o soaptube.apk -e amoled 
```
for normal dark mode

OR

```bat
java -jar builder.jar -b patches.jar -m integrations.apk -a youtube.apk -o soaptube.apk 
``` 
for amoled dark mode

# Known Issues:
- App crashes when ```Settings > ReVanced Settings > Layout Settings > Autoplay Button``` is toggled on
