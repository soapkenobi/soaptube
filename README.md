# SoapTube
Requires:
- Zulu JDK 17
- x64 OS
- Supported Youtube apk(Current=17.29.34); make sure apk is not bundle

## Table of content:
[Installation](#installation)
- [Preparation](#preparation)
- [Final Directory Structure]("#fd")

[Known Issues](#known_issues)

## Installation:
### Preparation:

- Install Azul JDK 17
- Clone this repository
- Rename your youtube apk to ```youtube.apk```
- Copy the ```youtube.apk``` to root directory of the cloned repository
<a name="fd"/>
### Final directory structure before build
![Directory](https://user-images.githubusercontent.com/80191638/183301613-26f480fb-a911-4f0b-9d21-4e5c4720badf.png)


### Building
To compile execute:

```bat
java -jar builder.jar -b patches.jar -m integrations.apk -a youtube.apk -o soaptube.apk -e amoled 
```
for normal dark mode

OR

```bat
java -jar builder.jar -b patches.jar -m integrations.apk -a youtube.apk -o soaptube.apk 
``` 
for amoled dark mode

<a name="known_issues"/>

## Known Issues:

- App crashes when ```Settings > ReVanced Settings > Layout Settings > Autoplay Button``` is toggled on
