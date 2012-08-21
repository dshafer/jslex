# jslex
Not very long ago, I was surprised and troubled to find that there was apparently no ready-made solution to my pressing need to transform arbritray text into [swedish chef](http://www.youtube.com/results?search_query=swedish+chef) dialect.  This is a problem that the unix world addressed decades ago with a little bit of [lex](http://en.wikipedia.org/wiki/Lex_programming_tool) magic, but somehow, tragically, unforgivably, front-end developers haven't had easy access to this important tool.

#### Obviously, somebody needed to do something.
`jslex` is my answer to this problem.  The design is informed somewhat by lex's input files, but I made no attempt at compatibility or feature-parity.  Basically, the features that exist are those that I needed to be able to borkify text.

## Usage
```javascript
var translator = Translate.compile_translator(borkborkbork);
console.log(translator.translate('Welcome.'); // prints "Velcume-a.  Bork Bork Bork!"
```

See [test_translate.html](https://github.com/dshafer/jslex/blob/master/test_translate.html) for a full example.