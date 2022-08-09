# SoapTube
### ![Banner](https://ondemand.bannerbear.com/signedurl/9K5qxXae32jEAGRDkj/image.jpg?modifications=W3sibmFtZSI6InJlcG8iLCJ0ZXh0IjoiQ2FwTWFjdGF2aXNoMjQxIC8gKnNvYXB0dWJlKiJ9LHsibmFtZSI6ImRlc2MiLCJ0ZXh0IjoiU29hcFR1YmUgaXMgYSBiZXR0ZXIgdmVyc2lvbiBvZiB0aGUgc3RvY2sgQW5kcm9pZCBZb3VUdWJlIGFwcCEgSW5jbHVkZXMgYWRibG9ja2luZywgYmFja2dyb3VuZCBwbGF5YmFjaywgYW5kIGxvdCBtb3JlKG5vdCBhZmZpbGlhdGVkIHdpdGggR29vZ2xlIGluYy4gb3IgWW91dHViZSkifSx7Im5hbWUiOiJhdmF0YXI1IiwiaGlkZSI6dHJ1ZX0seyJuYW1lIjoiYXZhdGFyNCIsImhpZGUiOnRydWV9LHsibmFtZSI6ImF2YXRhcjMiLCJoaWRlIjp0cnVlfSx7Im5hbWUiOiJhdmF0YXIyIiwiaGlkZSI6dHJ1ZX0seyJuYW1lIjoiYXZhdGFyMSIsImltYWdlX3VybCI6Imh0dHBzOi8vYXZhdGFycy5naXRodWJ1c2VyY29udGVudC5jb20vdS84MDE5MTYzOD92PTQifSx7Im5hbWUiOiJjb250cmlidXRvcnMiLCJ0ZXh0IjoiQ2FwTWFjdGF2aXNoMjQxIn0seyJuYW1lIjoic3RhcnMiLCJ0ZXh0IjoiMSJ9XQ&s=634a0d9b314c295007b134eabe20cf3e07f9d4d275ae3096f17a769173a43a30)

## Table of Content:
[Self Compile](#self-compile)
- [Requirements](#requirements)
- [Preparation](#preparation)
- [Final Directory Structure](#fd)
- [Building](#building)

[Known Issues](#known_issues)

## Self-Compile:

## Requirements:
- Access to Internet
- x64 OS
- Youtube apk; make sure apk is not bundle
- Basic command line knowledge

### Preparation:

- Install [Azul JDK 17](https://cdn.azul.com/zulu/bin/zulu17.36.13-ca-jdk17.0.4-win_x64.msi)
- Clone this repository
- Rename your youtube apk to ```youtube.apk```
- Copy the ```youtube.apk``` to root directory of the cloned repository
<a name="fd"/>

### Final directory structure before build
![Directory](https://user-images.githubusercontent.com/80191638/183302014-fa0f28d5-59aa-41f5-be13-33645d51bc1e.png)


### Building
To compile execute one of these in the directory where you cloned this repository:

```bat
java -jar builder.jar -b patches.jar -m integrations.apk -a youtube.apk -o soaptube.apk -e amoled -e hide-autoplay-button --experimental
```
for normal dark mode

OR

```bat
java -jar builder.jar -b patches.jar -m integrations.apk -a youtube.apk -o soaptube.apk -e hide-autoplay-button --experimental
``` 
for amoled dark mode

<a name="known_issues"/>

## Known Issues:

- ### ~App crashes when ```Settings > SoapTube Settings > Layout Settings > Autoplay Button``` is toggled on~
