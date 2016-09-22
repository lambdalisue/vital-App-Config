vital-App-Config
==============================================================================
[![Travis CI](https://img.shields.io/travis/lambdalisue/vital-App-Config/master.svg?style=flat-square&label=Travis%20CI)](https://travis-ci.org/lambdalisue/vital-App-Config)
[![AppVeyor](https://img.shields.io/appveyor/ci/lambdalisue/vital-App-Config/master.svg?style=flat-square&label=AppVeyor)](https://ci.appveyor.com/project/lambdalisue/vital-App-Config/branch/master)
![Version 1.0.0](https://img.shields.io/badge/version-1.0.0-yellow.svg?style=flat-square)
![Support Vim 7.4 or above](https://img.shields.io/badge/support-Vim%207.4%20or%20above-yellowgreen.svg?style=flat-square)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](LICENSE.md)
[![Doc](https://img.shields.io/badge/doc-%3Ah%20vital--App--Config-orange.svg?style=flat-square)](doc/vital-app-config.txt)


Install
-------------------------------------------------------------------------------

```vim
Plug 'lambdalisue/vital-App-Config'
```

And call the following to bundle this plugin

```vim
:Vitalize . +Vim.Prompt
```

Usage
-------------------------------------------------------------------------------

```vim
let s:Config = vital#vital#import('App.Config')

" Define the following only when the variable is missing
" - g:vital#foo#bar#foo = 1
" - g:vital#foo#bar#bar = 'bar'
" Useful to define default variables
call s:Config.define('vital#foo#bar', {
      \ 'foo': 1,
      \ 'bar': 'bar',
      \})
```
