---
layout: post
title: SublimeText3 설치 및 설정(Windows10)
---

본 포스트는 SublimeText3 설치 및 설정에 관련 된 방법을 서술한다.


### 1. Sublime Text 3 설치(windows 기준 설명)
 
> 1.  https://www.sublimetext.com/3 에 접근하여  OS 에 맞는 최신 버전의 Sublime Text를 다운로드 받는다.
  2.  다운로드 완료 후 설치 파일을 실행하며, 특별한 설정은 필요하지 않다.


[Sublime Text 3 다운로드 page](https://www.sublimetext.com/3 "다운로드 Url") 

### 2. Sublime Text 3 기본 설정
1. sublime Text console을 오픈한다. (Ctrl+`)
2. 아래의 내용을 복사하여 콘솔에서 실행한다.

```shell
import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

![Package Controller installation](sublime_install_01.png "title") 

