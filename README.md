Wercker box gox [![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://github.com/tcnksm/wercker-box-gox/blob/master/LICENCE)
====

[![wercker status](https://app.wercker.com/status/1e96bc8093f7b7ae1881c6dfb62157d3/m "wercker status")](https://app.wercker.com/project/bykey/1e96bc8093f7b7ae1881c6dfb62157d3)


This is [wercker](http://wercker.com/) box which is installed [mitchellh/gox](https://github.com/mitchellh/gox), cross-compiling golang project parallelly.

To build tool-chain, it takes long time, so we should pre-install it as box

## Usage

In the `wercker.yml` of your application use the following step definition:

```yaml
box: tcnksm/gox@1.4.1
```

## Box details

This box is based on Ubuntu 12.04 and inherited from [werkcer/golang@1.3.1](https://github.com/wercker/box-golang).

## Steps

You can use below step scripts they would work well with this box:

- [tcnksm/wercker-step-gox](https://github.com/tcnksm/wercker-step-gox) - Wercker step for mitchellh/gox, cross-compiling golang project parallelly
- [tcnksm/wercker-step-zip](https://github.com/tcnksm/wercker-step-zip) - Wercker step for packaging directories
- [tcnksm/wercker-step-ghr](https://github.com/tcnksm/wercker-step-ghr) - Wercker step for tcnksm/ghr, create Github Release and uploading artifacts

## Author

[tcnksm](https://github.com/tcnksm)
