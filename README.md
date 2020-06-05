# About this fork

I've updated the cwebp library and added the 'parameters' parameter to the method '.toNormalImage' and 'toWEBP'.

This is also posted in a topic on https://coderanch.com/ since its my first fork of a public project.

My thanks to 'biezhi' for allowing forks and coderanch for general help.

PS: This is my first fork, so Im sorry if I missed anything.


Example of new Usage:
```java
    public static void main(String args[]) throws IOException {
        String src = "A:\\Downloads\\image.jpg";
        String dest = "A:\\Downloads\\image.webp";
		String parameters = "-q 80 -resize 400 0 -z 9 -m 6 -mt";
        WebpIO.create().toWEBP(src, dest, parameters);
    }
```


# webp-io

The **webp-io** is convert normal image and `webp` file.

[![](https://img.shields.io/travis/biezhi/webp-io.svg)](https://travis-ci.org/biezhi/webp-io)
[![](https://img.shields.io/badge/license-Apache2-FF0080.svg)](https://github.com/biezhi/webp-io/blob/master/LICENSE)

## Usage

**Maven dependency**

```xml
<dependency>
    <groupId>io.github.biezhi</groupId>
    <artifactId>webp-io</artifactId>
    <version>0.0.5</version>
</dependency>
```

**API**

```java
String src  = "a.webp";
String dest = "a.png";
WebpIO.create().toNormalImage(src, dest);

WebpIO.create().toWEBP("hello.png", "hello.webp");
```


