jquery-sexy-placeholder
=======================

A sexier placeholder shim. Dress it up however you like.

[![Build Status](https://travis-ci.org/tylermauthe/jquery-sexy-placeholder.png?branch=master)](https://travis-ci.org/tylermauthe/jquery-sexy-placeholder)
[![Selenium Test Status](https://saucelabs.com/buildstatus/sexyplaceholder)](https://saucelabs.com/u/sexyplaceholder)

## Support
This plugin is tested with IE8 and IE9 on Windows 7. Might work with other browsers... If you find that it happens to work for your browser/platform, drop me a line an I'll add it to the list.

## Motivation
Other placeholder shims exist and they're very nice in their own way, but this plugin is unassuming and totally stylable. While some other plugins utilize an approach that sets the value in the input element to simulate a placeholder, this plugin uses a simple span element for greater stylability. `jquery-sexy-placeholder` makes no assumptions, it is totally submissive. If you can't seem to make up your mind about what you want from this plugin, then you lay back, relax, and let the plugin do all the work by using a predefined default method - more on this below.

## Usage
Say you've got a few input elements:
```html
  <input placholder="Username" type="text" />
  <input placholder="Password" type="password" />
  ...
```
You can initialize jquery-sexy-placeholder as easily as this: `$('input').sexyPlaceholder()`

Then style the css class `placeholder`: (taken from [WebKit Default User Agent Stylesheet](http://trac.webkit.org/browser/trunk/Source/WebCore/css/html.css))
```css
  .placeholder {
    position: absolute;
    top: 2px;
    left: 4px;
    font-size: 80%;
    word-spacing: -1px;
    color: #A9A9A9;
    pointer-events: none !important;
  }
```

## Defaults
If those CSS values look right to you and you don't really give a hoot about the styling, instead use `$('input').sexyPlaceholderDefaults()` and you'll have the same defaults set automatically.

## Testing
`jquery-sexy-plugin` uses Jasmine to ensure it stays sexy even after some crazy forking. Please ensure all pull requests for new features have proper tests and that any bug fixes or featre modifications do not fail the existing tests.

Please feel free to criticize, balk at or otherwise refactor the tests too, because I'm a testing `n00b`.

## License
Same license as jQuery, MIT.
