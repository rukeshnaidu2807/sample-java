# sample-java

[![build status][travis-image]][travis-url]

Macaca test sample for Java

[API Doc](//macacajs.github.io/wd.java/)

[gitter-url]: https://gitter.im/alibaba/macaca

[travis-image]: https://img.shields.io/travis/macaca-sample/sample-java.svg?style=flat-square
[travis-url]: https://travis-ci.org/macaca-sample/sample-java

## more docs 参考文章

[https://testerhome.com/junhe](https://testerhome.com/junhe)

## Test

Start macaca server

``` bash
$ macaca server --verbose
```

install mvn dependencies：

``` bash
$ mvn -s settings.xml clean install -Dmaven.test.skip=true
```

run test

``` bash
$ mvn -s settings.xml test -Dtest=macaca.client.AndroidSampleTest
```

## App Source Code

- [ios-app-bootstrap](//github.com/xudafeng/ios-app-bootstrap)
- [android-app-bootstrap](//github.com/xudafeng/android-app-bootstrap)

## RUN CI

when source code changes, run CI Samples

1. change current version : package.json
2. npm publish
3. run CI sample

## Problems

1. when you run iosSampleTest.java,you may meet this problem:


``` bash

ios_webkit_debug_proxy path: /usr/local/bin/ios_webkit_debug_proxy
Could not connect to lockdownd. Exiting.: Permission denied
Unable to attach f27bc6f301486418d3c81c04165cbd93143ec972 inspector
Invalid message _rpc_reportConnectedDriverList: <dict>
	<key>WIRDriverDictionaryKey</key>
	<dict>
	</dict>
</dict>

```

that's because you do not have permission for ios_webkit_debug_proxy, you can solve this problem by this:

1. refer to: [http://stackoverflow.com/questions/39035415/ideviceinstaller-fails-with-could-not-connect-to-lockdownd-exiting](http://stackoverflow.com/questions/39035415/ideviceinstaller-fails-with-could-not-connect-to-lockdownd-exiting)

2. if the problem still exists ,upgrade ios-ios-webkit-debug-proxy(my version is ios-webkit-debug-proxy-1.7.1)


``` bash
$ brew upgrade ios-webkit-debug-proxy
```

<!-- GITCONTRIBUTOR_START -->

## Contributors

|[<img src="https://avatars2.githubusercontent.com/u/5734727?v=4" width="100px;"/><br/><sub><b>Yinxl</b></sub>](https://github.com/Yinxl)<br/>|[<img src="https://avatars1.githubusercontent.com/u/1011681?v=4" width="100px;"/><br/><sub><b>xudafeng</b></sub>](https://github.com/xudafeng)<br/>|[<img src="https://avatars1.githubusercontent.com/u/17233599?v=4" width="100px;"/><br/><sub><b>Chan-Chun</b></sub>](https://github.com/Chan-Chun)<br/>
| :---: | :---: | :---: |


This project follows the git-contributor [spec](https://github.com/xudafeng/git-contributor), auto upated at `Sat Apr 21 2018 17:28:19 GMT+0800`.

<!-- GITCONTRIBUTOR_END -->

## License



thisa is harish

The MIT License (MIT)
