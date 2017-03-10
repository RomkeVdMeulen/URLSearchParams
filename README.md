# URLSearchParams

## DEPRECATED (2017-03-10) ##

With release 2.2.1 of TypeScript, `interface URLSearchParams` has [finally landed in the standard DOM library](https://github.com/Microsoft/TypeScript/blob/v2.2.1/lib/lib.dom.d.ts#L13858). To include it in your build, upgrade to TypeScript 2.2.1 or higher and check your `tsconfig.json` to make sure the DOM lib is included in your build (by default it is).

### Cleanup ###

To remove this library from your typings execute:

```
typings uninstall url-search-params-typing --global --save
```

## About this ##

By some unfortunate timing, the typings for the [URLSearchParams](URLSearchParams) interface, part of the
[whatwg URL spec](https://url.spec.whatwg.org/#urlsearchparams), aren't available anywhere, even though some code is
[already using it](https://github.com/DefinitelyTyped/DefinitelyTyped/blob/dcb46429c820bac49c31ef9f4ee4154cac01fb80/whatwg-fetch/whatwg-fetch.d.ts#L31).

This repo can be used as a temporary patch until the interface is added to a standard library. To install:

```
typings install github:RomkeVdMeulen/URLSearchParams --global --save
```
