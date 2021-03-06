# jQuery - transitionend for CSS animations

Monkeypatch the `jQuery.fn.on` function, so we can just use

```javascript
$('.my-element').one('transitionend', function(){
  console.log('Finished animation');
});
```

instead of

```javascript
$('.my-element').one('webkitTransitionEnd oTransitionEnd msTransitionEnd transitionend', function(){
  console.log('Finished animation');
});
```

Available through Bower: `bower install jquery-transitionend`.

## Running tests

Just open the file `test/index.html` in your target browser.

## Maintainer

- Nando Vieira - <http://nandovieira.com.br>

## License

(The MIT License)

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
