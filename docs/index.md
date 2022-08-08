# SoapTube
### ![Banner](https://user-images.githubusercontent.com/80191638/183302385-0714ffc2-8c60-4c90-8f6e-342c8eebab51.jpg)

[Download Compiled Binaries](http://github.com/CapMactavish241/soaptube/releases){: .btn {
  -webkit-border-radius: 7;
  -moz-border-radius: 7;
  border-radius: 7px;
  font-family: Arial;
  color: #ffffff;
  font-size: 20px;
  background: #4e5961;
  padding: 10px 20px 10px 20px;
  text-decoration: none;
}

.btn:hover {
  background: #292929;
  text-decoration: none;
}}

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
