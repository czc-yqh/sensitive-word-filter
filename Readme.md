
# sensitive-word-filter2
[![NPM version][npm-image]][npm-url]
[![Build Status][travis-image]][travis-url]
[![Downloads][downloads-image]][downloads-url]

### Introduction
A simple&basic text filter that is under censor of GFW, with DFA.

为nodejs提供的简单GFW敏感词过滤器，使用DFA实现。

### Install

$ npm install sensitive-word-filter

### Usage

    var wc = require('sensitive-word-filter')
    var string = "习近平大大,Ur so sexy babe!"
    string = wc.filter(string) 
    console.log(string) // ***大大,Ur so ***y babe!

If you want to add key words of your own, simply add them to the end of 'keywords' file, one word per line.

在'keywords'文件末尾增加自定义敏感词，每行一个。

### Performance

Under 1ms for a 10-20 words sentence. Around 10ms for 1000 words.

10-20字的短句在1ms以内替换完成，1000字左右需要10ms左右



### Thanks
Keyword list from https://github.com/observerss/textfilter

### License
MIT

[npm-url]: https://npmjs.org/package/sensitive-word-filter
[npm-image]: https://img.shields.io/npm/v/sensitive-word-filter.svg 

[travis-url]: https://travis-ci.org/gaohuifeng/sensitive-word-filter
[travis-image]: https://travis-ci.org/gaohuifeng/sensitive-word-filter.svg?branch=master

[downloads-url]: https://npmjs.org/package/sensitive-word-filter
[downloads-image]: https://img.shields.io/github/downloads/atom/atom/latest/total.svg
