### ![Banner](https://user-images.githubusercontent.com/80191638/183302385-0714ffc2-8c60-4c90-8f6e-342c8eebab51.jpg)

# SoapTube
Requires:
- Zulu JDK 17
- x64 OS
- Supported Youtube apk(Current=17.29.34); make sure apk is not bundle

## Table of content:
[Installation](#installation)
- [Preparation](#preparation)
- [Final Directory Structure](#fd)
- [Building](#building)

[Known Issues](#known_issues)

## Installation:
### Preparation:

- Install Azul JDK 17
- Clone this repository
- Rename your youtube apk to ```youtube.apk```
- Copy the ```youtube.apk``` to root directory of the cloned repository
<a name="fd"/>

### Final directory structure before build
![Directory](https://user-images.githubusercontent.com/80191638/183302014-fa0f28d5-59aa-41f5-be13-33645d51bc1e.png)


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
