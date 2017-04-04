# api documentation for  [gulp-markdown (v1.2.0)](https://github.com/sindresorhus/gulp-markdown)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-markdown.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-markdown) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-markdown.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-markdown)
#### Markdown to HTML

[![NPM](https://nodei.co/npm/gulp-markdown.png?downloads=true)](https://www.npmjs.com/package/gulp-markdown)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-markdown/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gulp-markdown_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-markdown/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-markdown/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-markdown/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Sindre Sorhus",
        "email": "sindresorhus@gmail.com",
        "url": "http://sindresorhus.com"
    },
    "bugs": {
        "url": "https://github.com/sindresorhus/gulp-markdown/issues"
    },
    "dependencies": {
        "gulp-util": "^3.0.0",
        "marked": "^0.3.2",
        "through2": "^2.0.0"
    },
    "description": "Markdown to HTML",
    "devDependencies": {
        "mocha": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "37cdc61379fb039841fa6cab4984a8e79128a772",
        "tarball": "https://registry.npmjs.org/gulp-markdown/-/gulp-markdown-1.2.0.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "files": [
        "index.js"
    ],
    "gitHead": "a4b1d4532ab54c008b1b3cafc35cd1e937941d6b",
    "homepage": "https://github.com/sindresorhus/gulp-markdown",
    "keywords": [
        "gulpplugin",
        "markdown",
        "marked",
        "md",
        "compile",
        "convert",
        "markup",
        "html"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "sindresorhus",
            "email": "sindresorhus@gmail.com"
        }
    ],
    "name": "gulp-markdown",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/sindresorhus/gulp-markdown.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "version": "1.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-markdown](#apidoc.module.gulp-markdown)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.</span>marked (src, opt, callback)](#apidoc.element.gulp-markdown.marked)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.</span>marked.InlineLexer (links, options)](#apidoc.element.gulp-markdown.marked.InlineLexer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.</span>marked.Lexer (options)](#apidoc.element.gulp-markdown.marked.Lexer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.</span>marked.Parser (options)](#apidoc.element.gulp-markdown.marked.Parser)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.</span>marked.Renderer (options)](#apidoc.element.gulp-markdown.marked.Renderer)
1.  object <span class="apidocSignatureSpan">gulp-markdown.</span>marked.InlineLexer.prototype
1.  object <span class="apidocSignatureSpan">gulp-markdown.</span>marked.Lexer.prototype
1.  object <span class="apidocSignatureSpan">gulp-markdown.</span>marked.Parser.prototype
1.  object <span class="apidocSignatureSpan">gulp-markdown.</span>marked.Renderer.prototype

#### [module gulp-markdown.marked](#apidoc.module.gulp-markdown.marked)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.</span>marked (src, opt, callback)](#apidoc.element.gulp-markdown.marked.marked)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>InlineLexer (links, options)](#apidoc.element.gulp-markdown.marked.InlineLexer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Lexer (options)](#apidoc.element.gulp-markdown.marked.Lexer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Parser (options)](#apidoc.element.gulp-markdown.marked.Parser)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Renderer (options)](#apidoc.element.gulp-markdown.marked.Renderer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>inlineLexer (src, links, options)](#apidoc.element.gulp-markdown.marked.inlineLexer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>lexer (src, options)](#apidoc.element.gulp-markdown.marked.lexer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>options (opt)](#apidoc.element.gulp-markdown.marked.options)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>parse (src, opt, callback)](#apidoc.element.gulp-markdown.marked.parse)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>parser (src, options, renderer)](#apidoc.element.gulp-markdown.marked.parser)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>setOptions (opt)](#apidoc.element.gulp-markdown.marked.setOptions)
1.  object <span class="apidocSignatureSpan">gulp-markdown.marked.</span>defaults

#### [module gulp-markdown.marked.InlineLexer](#apidoc.module.gulp-markdown.marked.InlineLexer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>InlineLexer (links, options)](#apidoc.element.gulp-markdown.marked.InlineLexer.InlineLexer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.InlineLexer.</span>output (src, links, options)](#apidoc.element.gulp-markdown.marked.InlineLexer.output)
1.  object <span class="apidocSignatureSpan">gulp-markdown.marked.InlineLexer.</span>rules

#### [module gulp-markdown.marked.InlineLexer.prototype](#apidoc.module.gulp-markdown.marked.InlineLexer.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.InlineLexer.prototype.</span>mangle (text)](#apidoc.element.gulp-markdown.marked.InlineLexer.prototype.mangle)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.InlineLexer.prototype.</span>output (src)](#apidoc.element.gulp-markdown.marked.InlineLexer.prototype.output)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.InlineLexer.prototype.</span>outputLink (cap, link)](#apidoc.element.gulp-markdown.marked.InlineLexer.prototype.outputLink)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.InlineLexer.prototype.</span>smartypants (text)](#apidoc.element.gulp-markdown.marked.InlineLexer.prototype.smartypants)

#### [module gulp-markdown.marked.Lexer](#apidoc.module.gulp-markdown.marked.Lexer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Lexer (options)](#apidoc.element.gulp-markdown.marked.Lexer.Lexer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Lexer.</span>lex (src, options)](#apidoc.element.gulp-markdown.marked.Lexer.lex)
1.  object <span class="apidocSignatureSpan">gulp-markdown.marked.Lexer.</span>rules

#### [module gulp-markdown.marked.Lexer.prototype](#apidoc.module.gulp-markdown.marked.Lexer.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Lexer.prototype.</span>lex (src)](#apidoc.element.gulp-markdown.marked.Lexer.prototype.lex)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Lexer.prototype.</span>token (src, top, bq)](#apidoc.element.gulp-markdown.marked.Lexer.prototype.token)

#### [module gulp-markdown.marked.Parser](#apidoc.module.gulp-markdown.marked.Parser)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Parser (options)](#apidoc.element.gulp-markdown.marked.Parser.Parser)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.</span>parse (src, options, renderer)](#apidoc.element.gulp-markdown.marked.Parser.parse)

#### [module gulp-markdown.marked.Parser.prototype](#apidoc.module.gulp-markdown.marked.Parser.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.prototype.</span>next ()](#apidoc.element.gulp-markdown.marked.Parser.prototype.next)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.prototype.</span>parse (src)](#apidoc.element.gulp-markdown.marked.Parser.prototype.parse)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.prototype.</span>parseText ()](#apidoc.element.gulp-markdown.marked.Parser.prototype.parseText)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.prototype.</span>peek ()](#apidoc.element.gulp-markdown.marked.Parser.prototype.peek)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.prototype.</span>tok ()](#apidoc.element.gulp-markdown.marked.Parser.prototype.tok)

#### [module gulp-markdown.marked.Renderer](#apidoc.module.gulp-markdown.marked.Renderer)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Renderer (options)](#apidoc.element.gulp-markdown.marked.Renderer.Renderer)

#### [module gulp-markdown.marked.Renderer.prototype](#apidoc.module.gulp-markdown.marked.Renderer.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>blockquote (quote)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.blockquote)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>br ()](#apidoc.element.gulp-markdown.marked.Renderer.prototype.br)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>code (code, lang, escaped)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.code)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>codespan (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.codespan)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>del (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.del)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>em (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.em)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>heading (text, level, raw)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.heading)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>hr ()](#apidoc.element.gulp-markdown.marked.Renderer.prototype.hr)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>html (html)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.html)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>image (href, title, text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.image)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>link (href, title, text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.link)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>list (body, ordered)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.list)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>listitem (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.listitem)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>paragraph (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.paragraph)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>strong (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.strong)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>table (header, body)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.table)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>tablecell (content, flags)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.tablecell)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>tablerow (content)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.tablerow)
1.  [function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>text (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.text)



# <a name="apidoc.module.gulp-markdown"></a>[module gulp-markdown](#apidoc.module.gulp-markdown)

#### <a name="apidoc.element.gulp-markdown.marked"></a>[function <span class="apidocSignatureSpan">gulp-markdown.</span>marked (src, opt, callback)](#apidoc.element.gulp-markdown.marked)
- description and source-code
```javascript
function marked(src, opt, callback) {
  if (callback || typeof opt === 'function') {
    if (!callback) {
      callback = opt;
      opt = null;
    }

    opt = merge({}, marked.defaults, opt || {});

    var highlight = opt.highlight
      , tokens
      , pending
      , i = 0;

    try {
      tokens = Lexer.lex(src, opt)
    } catch (e) {
      return callback(e);
    }

    pending = tokens.length;

    var done = function(err) {
      if (err) {
        opt.highlight = highlight;
        return callback(err);
      }

      var out;

      try {
        out = Parser.parse(tokens, opt);
      } catch (e) {
        err = e;
      }

      opt.highlight = highlight;

      return err
        ? callback(err)
        : callback(null, out);
    };

    if (!highlight || highlight.length < 3) {
      return done();
    }

    delete opt.highlight;

    if (!pending) return done();

    for (; i < tokens.length; i++) {
      (function(token) {
        if (token.type !== 'code') {
          return --pending || done();
        }
        return highlight(token.text, token.lang, function(err, code) {
          if (err) return done(err);
          if (code == null || code === token.text) {
            return --pending || done();
          }
          token.text = code;
          token.escaped = true;
          --pending || done();
        });
      })(tokens[i]);
    }

    return;
  }
  try {
    if (opt) opt = merge({}, marked.defaults, opt);
    return Parser.parse(Lexer.lex(src, opt), opt);
  } catch (e) {
    e.message += '\nPlease report this to https://github.com/chjj/marked.';
    if ((opt || marked.defaults).silent) {
      return '<p>An error occured:</p><pre>'
        + escape(e.message + '', true)
        + '</pre>';
    }
    throw e;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.InlineLexer"></a>[function <span class="apidocSignatureSpan">gulp-markdown.</span>marked.InlineLexer (links, options)](#apidoc.element.gulp-markdown.marked.InlineLexer)
- description and source-code
```javascript
function InlineLexer(links, options) {
  this.options = options || marked.defaults;
  this.links = links;
  this.rules = inline.normal;
  this.renderer = this.options.renderer || new Renderer;
  this.renderer.options = this.options;

  if (!this.links) {
    throw new
      Error('Tokens array requires a 'links' property.');
  }

  if (this.options.gfm) {
    if (this.options.breaks) {
      this.rules = inline.breaks;
    } else {
      this.rules = inline.gfm;
    }
  } else if (this.options.pedantic) {
    this.rules = inline.pedantic;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Lexer"></a>[function <span class="apidocSignatureSpan">gulp-markdown.</span>marked.Lexer (options)](#apidoc.element.gulp-markdown.marked.Lexer)
- description and source-code
```javascript
function Lexer(options) {
  this.tokens = [];
  this.tokens.links = {};
  this.options = options || marked.defaults;
  this.rules = block.normal;

  if (this.options.gfm) {
    if (this.options.tables) {
      this.rules = block.tables;
    } else {
      this.rules = block.gfm;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Parser"></a>[function <span class="apidocSignatureSpan">gulp-markdown.</span>marked.Parser (options)](#apidoc.element.gulp-markdown.marked.Parser)
- description and source-code
```javascript
function Parser(options) {
  this.tokens = [];
  this.token = null;
  this.options = options || marked.defaults;
  this.options.renderer = this.options.renderer || new Renderer;
  this.renderer = this.options.renderer;
  this.renderer.options = this.options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer"></a>[function <span class="apidocSignatureSpan">gulp-markdown.</span>marked.Renderer (options)](#apidoc.element.gulp-markdown.marked.Renderer)
- description and source-code
```javascript
function Renderer(options) {
  this.options = options || {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-markdown.marked"></a>[module gulp-markdown.marked](#apidoc.module.gulp-markdown.marked)

#### <a name="apidoc.element.gulp-markdown.marked.marked"></a>[function <span class="apidocSignatureSpan">gulp-markdown.</span>marked (src, opt, callback)](#apidoc.element.gulp-markdown.marked.marked)
- description and source-code
```javascript
function marked(src, opt, callback) {
  if (callback || typeof opt === 'function') {
    if (!callback) {
      callback = opt;
      opt = null;
    }

    opt = merge({}, marked.defaults, opt || {});

    var highlight = opt.highlight
      , tokens
      , pending
      , i = 0;

    try {
      tokens = Lexer.lex(src, opt)
    } catch (e) {
      return callback(e);
    }

    pending = tokens.length;

    var done = function(err) {
      if (err) {
        opt.highlight = highlight;
        return callback(err);
      }

      var out;

      try {
        out = Parser.parse(tokens, opt);
      } catch (e) {
        err = e;
      }

      opt.highlight = highlight;

      return err
        ? callback(err)
        : callback(null, out);
    };

    if (!highlight || highlight.length < 3) {
      return done();
    }

    delete opt.highlight;

    if (!pending) return done();

    for (; i < tokens.length; i++) {
      (function(token) {
        if (token.type !== 'code') {
          return --pending || done();
        }
        return highlight(token.text, token.lang, function(err, code) {
          if (err) return done(err);
          if (code == null || code === token.text) {
            return --pending || done();
          }
          token.text = code;
          token.escaped = true;
          --pending || done();
        });
      })(tokens[i]);
    }

    return;
  }
  try {
    if (opt) opt = merge({}, marked.defaults, opt);
    return Parser.parse(Lexer.lex(src, opt), opt);
  } catch (e) {
    e.message += '\nPlease report this to https://github.com/chjj/marked.';
    if ((opt || marked.defaults).silent) {
      return '<p>An error occured:</p><pre>'
        + escape(e.message + '', true)
        + '</pre>';
    }
    throw e;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.InlineLexer"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>InlineLexer (links, options)](#apidoc.element.gulp-markdown.marked.InlineLexer)
- description and source-code
```javascript
function InlineLexer(links, options) {
  this.options = options || marked.defaults;
  this.links = links;
  this.rules = inline.normal;
  this.renderer = this.options.renderer || new Renderer;
  this.renderer.options = this.options;

  if (!this.links) {
    throw new
      Error('Tokens array requires a 'links' property.');
  }

  if (this.options.gfm) {
    if (this.options.breaks) {
      this.rules = inline.breaks;
    } else {
      this.rules = inline.gfm;
    }
  } else if (this.options.pedantic) {
    this.rules = inline.pedantic;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Lexer"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Lexer (options)](#apidoc.element.gulp-markdown.marked.Lexer)
- description and source-code
```javascript
function Lexer(options) {
  this.tokens = [];
  this.tokens.links = {};
  this.options = options || marked.defaults;
  this.rules = block.normal;

  if (this.options.gfm) {
    if (this.options.tables) {
      this.rules = block.tables;
    } else {
      this.rules = block.gfm;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Parser"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Parser (options)](#apidoc.element.gulp-markdown.marked.Parser)
- description and source-code
```javascript
function Parser(options) {
  this.tokens = [];
  this.token = null;
  this.options = options || marked.defaults;
  this.options.renderer = this.options.renderer || new Renderer;
  this.renderer = this.options.renderer;
  this.renderer.options = this.options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Renderer (options)](#apidoc.element.gulp-markdown.marked.Renderer)
- description and source-code
```javascript
function Renderer(options) {
  this.options = options || {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.inlineLexer"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>inlineLexer (src, links, options)](#apidoc.element.gulp-markdown.marked.inlineLexer)
- description and source-code
```javascript
inlineLexer = function (src, links, options) {
  var inline = new InlineLexer(links, options);
  return inline.output(src);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.lexer"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>lexer (src, options)](#apidoc.element.gulp-markdown.marked.lexer)
- description and source-code
```javascript
lexer = function (src, options) {
  var lexer = new Lexer(options);
  return lexer.lex(src);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.options"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>options (opt)](#apidoc.element.gulp-markdown.marked.options)
- description and source-code
```javascript
options = function (opt) {
  merge(marked.defaults, opt);
  return marked;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.parse"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>parse (src, opt, callback)](#apidoc.element.gulp-markdown.marked.parse)
- description and source-code
```javascript
function marked(src, opt, callback) {
  if (callback || typeof opt === 'function') {
    if (!callback) {
      callback = opt;
      opt = null;
    }

    opt = merge({}, marked.defaults, opt || {});

    var highlight = opt.highlight
      , tokens
      , pending
      , i = 0;

    try {
      tokens = Lexer.lex(src, opt)
    } catch (e) {
      return callback(e);
    }

    pending = tokens.length;

    var done = function(err) {
      if (err) {
        opt.highlight = highlight;
        return callback(err);
      }

      var out;

      try {
        out = Parser.parse(tokens, opt);
      } catch (e) {
        err = e;
      }

      opt.highlight = highlight;

      return err
        ? callback(err)
        : callback(null, out);
    };

    if (!highlight || highlight.length < 3) {
      return done();
    }

    delete opt.highlight;

    if (!pending) return done();

    for (; i < tokens.length; i++) {
      (function(token) {
        if (token.type !== 'code') {
          return --pending || done();
        }
        return highlight(token.text, token.lang, function(err, code) {
          if (err) return done(err);
          if (code == null || code === token.text) {
            return --pending || done();
          }
          token.text = code;
          token.escaped = true;
          --pending || done();
        });
      })(tokens[i]);
    }

    return;
  }
  try {
    if (opt) opt = merge({}, marked.defaults, opt);
    return Parser.parse(Lexer.lex(src, opt), opt);
  } catch (e) {
    e.message += '\nPlease report this to https://github.com/chjj/marked.';
    if ((opt || marked.defaults).silent) {
      return '<p>An error occured:</p><pre>'
        + escape(e.message + '', true)
        + '</pre>';
    }
    throw e;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.parser"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>parser (src, options, renderer)](#apidoc.element.gulp-markdown.marked.parser)
- description and source-code
```javascript
parser = function (src, options, renderer) {
  var parser = new Parser(options, renderer);
  return parser.parse(src);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.setOptions"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>setOptions (opt)](#apidoc.element.gulp-markdown.marked.setOptions)
- description and source-code
```javascript
setOptions = function (opt) {
  merge(marked.defaults, opt);
  return marked;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-markdown.marked.InlineLexer"></a>[module gulp-markdown.marked.InlineLexer](#apidoc.module.gulp-markdown.marked.InlineLexer)

#### <a name="apidoc.element.gulp-markdown.marked.InlineLexer.InlineLexer"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>InlineLexer (links, options)](#apidoc.element.gulp-markdown.marked.InlineLexer.InlineLexer)
- description and source-code
```javascript
function InlineLexer(links, options) {
  this.options = options || marked.defaults;
  this.links = links;
  this.rules = inline.normal;
  this.renderer = this.options.renderer || new Renderer;
  this.renderer.options = this.options;

  if (!this.links) {
    throw new
      Error('Tokens array requires a 'links' property.');
  }

  if (this.options.gfm) {
    if (this.options.breaks) {
      this.rules = inline.breaks;
    } else {
      this.rules = inline.gfm;
    }
  } else if (this.options.pedantic) {
    this.rules = inline.pedantic;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.InlineLexer.output"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.InlineLexer.</span>output (src, links, options)](#apidoc.element.gulp-markdown.marked.InlineLexer.output)
- description and source-code
```javascript
output = function (src, links, options) {
  var inline = new InlineLexer(links, options);
  return inline.output(src);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-markdown.marked.InlineLexer.prototype"></a>[module gulp-markdown.marked.InlineLexer.prototype](#apidoc.module.gulp-markdown.marked.InlineLexer.prototype)

#### <a name="apidoc.element.gulp-markdown.marked.InlineLexer.prototype.mangle"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.InlineLexer.prototype.</span>mangle (text)](#apidoc.element.gulp-markdown.marked.InlineLexer.prototype.mangle)
- description and source-code
```javascript
mangle = function (text) {
  if (!this.options.mangle) return text;
  var out = ''
    , l = text.length
    , i = 0
    , ch;

  for (; i < l; i++) {
    ch = text.charCodeAt(i);
    if (Math.random() > 0.5) {
      ch = 'x' + ch.toString(16);
    }
    out += '&#' + ch + ';';
  }

  return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.InlineLexer.prototype.output"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.InlineLexer.prototype.</span>output (src)](#apidoc.element.gulp-markdown.marked.InlineLexer.prototype.output)
- description and source-code
```javascript
output = function (src) {
  var out = ''
    , link
    , text
    , href
    , cap;

  while (src) {
    // escape
    if (cap = this.rules.escape.exec(src)) {
      src = src.substring(cap[0].length);
      out += cap[1];
      continue;
    }

    // autolink
    if (cap = this.rules.autolink.exec(src)) {
      src = src.substring(cap[0].length);
      if (cap[2] === '@') {
        text = cap[1].charAt(6) === ':'
          ? this.mangle(cap[1].substring(7))
          : this.mangle(cap[1]);
        href = this.mangle('mailto:') + text;
      } else {
        text = escape(cap[1]);
        href = text;
      }
      out += this.renderer.link(href, null, text);
      continue;
    }

    // url (gfm)
    if (!this.inLink && (cap = this.rules.url.exec(src))) {
      src = src.substring(cap[0].length);
      text = escape(cap[1]);
      href = text;
      out += this.renderer.link(href, null, text);
      continue;
    }

    // tag
    if (cap = this.rules.tag.exec(src)) {
      if (!this.inLink && /^<a /i.test(cap[0])) {
        this.inLink = true;
      } else if (this.inLink && /^<\/a>/i.test(cap[0])) {
        this.inLink = false;
      }
      src = src.substring(cap[0].length);
      out += this.options.sanitize
        ? this.options.sanitizer
          ? this.options.sanitizer(cap[0])
          : escape(cap[0])
        : cap[0]
      continue;
    }

    // link
    if (cap = this.rules.link.exec(src)) {
      src = src.substring(cap[0].length);
      this.inLink = true;
      out += this.outputLink(cap, {
        href: cap[2],
        title: cap[3]
      });
      this.inLink = false;
      continue;
    }

    // reflink, nolink
    if ((cap = this.rules.reflink.exec(src))
        || (cap = this.rules.nolink.exec(src))) {
      src = src.substring(cap[0].length);
      link = (cap[2] || cap[1]).replace(/\s+/g, ' ');
      link = this.links[link.toLowerCase()];
      if (!link || !link.href) {
        out += cap[0].charAt(0);
        src = cap[0].substring(1) + src;
        continue;
      }
      this.inLink = true;
      out += this.outputLink(cap, link);
      this.inLink = false;
      continue;
    }

    // strong
    if (cap = this.rules.strong.exec(src)) {
      src = src.substring(cap[0].length);
      out += this.renderer.strong(this.output(cap[2] || cap[1]));
      continue;
    }

    // em
    if (cap = this.rules.em.exec(src)) {
      src = src.substring(cap[0].length);
      out += this.renderer.em(this.output(cap[2] || cap[1]));
      continue;
    }

    // code
    if (cap = this.rules.code.exec(src)) {
      src = src.substring(cap[0].length);
      out += this.renderer.codespan(escape(cap[2], true));
      continue;
    }

    // br
    if (cap = this.rules.br.exec(src)) {
      src = src.substring(cap[0].length);
      out += this.renderer.br();
      continue;
    }

    // del (gfm)
    if (cap = this.rules.del.exec(src)) {
      src = src.substring(cap[0].length);
      out += this.renderer.del(this.output(cap[1]));
      continue;
    }

    // text
    if (cap = this.rules.text.exec(src)) {
      src = src.substring(cap[0].length);
      out += this.renderer.text(escape(this.smartypants(cap[0])));
      continue;
    }

    if (src) {
      throw new
        Error('Infinite loop on byte: ' + src.charCodeAt(0));
    }
  }

  return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.InlineLexer.prototype.outputLink"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.InlineLexer.prototype.</span>outputLink (cap, link)](#apidoc.element.gulp-markdown.marked.InlineLexer.prototype.outputLink)
- description and source-code
```javascript
outputLink = function (cap, link) {
  var href = escape(link.href)
    , title = link.title ? escape(link.title) : null;

  return cap[0].charAt(0) !== '!'
    ? this.renderer.link(href, title, this.output(cap[1]))
    : this.renderer.image(href, title, escape(cap[1]));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.InlineLexer.prototype.smartypants"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.InlineLexer.prototype.</span>smartypants (text)](#apidoc.element.gulp-markdown.marked.InlineLexer.prototype.smartypants)
- description and source-code
```javascript
smartypants = function (text) {
  if (!this.options.smartypants) return text;
  return text
    // em-dashes
    .replace(/---/g, '\u2014')
    // en-dashes
    .replace(/--/g, '\u2013')
    // opening singles
    .replace(/(^|[-\u2014/(\[{"\s])'/g, '$1\u2018')
    // closing singles & apostrophes
    .replace(/'/g, '\u2019')
    // opening doubles
    .replace(/(^|[-\u2014/(\[{\u2018\s])"/g, '$1\u201c')
    // closing doubles
    .replace(/"/g, '\u201d')
    // ellipses
    .replace(/\.{3}/g, '\u2026');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-markdown.marked.Lexer"></a>[module gulp-markdown.marked.Lexer](#apidoc.module.gulp-markdown.marked.Lexer)

#### <a name="apidoc.element.gulp-markdown.marked.Lexer.Lexer"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Lexer (options)](#apidoc.element.gulp-markdown.marked.Lexer.Lexer)
- description and source-code
```javascript
function Lexer(options) {
  this.tokens = [];
  this.tokens.links = {};
  this.options = options || marked.defaults;
  this.rules = block.normal;

  if (this.options.gfm) {
    if (this.options.tables) {
      this.rules = block.tables;
    } else {
      this.rules = block.gfm;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Lexer.lex"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Lexer.</span>lex (src, options)](#apidoc.element.gulp-markdown.marked.Lexer.lex)
- description and source-code
```javascript
lex = function (src, options) {
  var lexer = new Lexer(options);
  return lexer.lex(src);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-markdown.marked.Lexer.prototype"></a>[module gulp-markdown.marked.Lexer.prototype](#apidoc.module.gulp-markdown.marked.Lexer.prototype)

#### <a name="apidoc.element.gulp-markdown.marked.Lexer.prototype.lex"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Lexer.prototype.</span>lex (src)](#apidoc.element.gulp-markdown.marked.Lexer.prototype.lex)
- description and source-code
```javascript
lex = function (src) {
  src = src
    .replace(/\r\n|\r/g, '\n')
    .replace(/\t/g, '    ')
    .replace(/\u00a0/g, ' ')
    .replace(/\u2424/g, '\n');

  return this.token(src, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Lexer.prototype.token"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Lexer.prototype.</span>token (src, top, bq)](#apidoc.element.gulp-markdown.marked.Lexer.prototype.token)
- description and source-code
```javascript
token = function (src, top, bq) {
  var src = src.replace(/^ +$/gm, '')
    , next
    , loose
    , cap
    , bull
    , b
    , item
    , space
    , i
    , l;

  while (src) {
    // newline
    if (cap = this.rules.newline.exec(src)) {
      src = src.substring(cap[0].length);
      if (cap[0].length > 1) {
        this.tokens.push({
          type: 'space'
        });
      }
    }

    // code
    if (cap = this.rules.code.exec(src)) {
      src = src.substring(cap[0].length);
      cap = cap[0].replace(/^ {4}/gm, '');
      this.tokens.push({
        type: 'code',
        text: !this.options.pedantic
          ? cap.replace(/\n+$/, '')
          : cap
      });
      continue;
    }

    // fences (gfm)
    if (cap = this.rules.fences.exec(src)) {
      src = src.substring(cap[0].length);
      this.tokens.push({
        type: 'code',
        lang: cap[2],
        text: cap[3] || ''
      });
      continue;
    }

    // heading
    if (cap = this.rules.heading.exec(src)) {
      src = src.substring(cap[0].length);
      this.tokens.push({
        type: 'heading',
        depth: cap[1].length,
        text: cap[2]
      });
      continue;
    }

    // table no leading pipe (gfm)
    if (top && (cap = this.rules.nptable.exec(src))) {
      src = src.substring(cap[0].length);

      item = {
        type: 'table',
        header: cap[1].replace(/^ *| *\| *$/g, '').split(/ *\| */),
        align: cap[2].replace(/^ *|\| *$/g, '').split(/ *\| */),
        cells: cap[3].replace(/\n$/, '').split('\n')
      };

      for (i = 0; i < item.align.length; i++) {
        if (/^ *-+: *$/.test(item.align[i])) {
          item.align[i] = 'right';
        } else if (/^ *:-+: *$/.test(item.align[i])) {
          item.align[i] = 'center';
        } else if (/^ *:-+ *$/.test(item.align[i])) {
          item.align[i] = 'left';
        } else {
          item.align[i] = null;
        }
      }

      for (i = 0; i < item.cells.length; i++) {
        item.cells[i] = item.cells[i].split(/ *\| */);
      }

      this.tokens.push(item);

      continue;
    }

    // lheading
    if (cap = this.rules.lheading.exec(src)) {
      src = src.substring(cap[0].length);
      this.tokens.push({
        type: 'heading',
        depth: cap[2] === '=' ? 1 : 2,
        text: cap[1]
      });
      continue;
    }

    // hr
    if (cap = this.rules.hr.exec(src)) {
      src = src.substring(cap[0].length);
      this.tokens.push({
        type: 'hr'
      });
      continue;
    }

    // blockquote
    if (cap = this.rules.blockquote.exec(src)) {
      src = src.substring(cap[0].length);

      this.tokens.push({
        type: 'blockquote_start'
      });

      cap = cap[0].replace(/^ *> ?/gm, '');

      // Pass 'top' to keep the current
      // "toplevel" state. This is exactly
      // how markdown.pl works.
      this.token(cap, top, true);

      this.tokens.push({
        type: 'blockquote_end'
      });

      continue;
    }

    // list
    if (cap = this.rules.list.exec(src)) {
      src = src.substring(cap[0].length);
      bull = cap[2];

      this.tokens.push({
        type: 'list_start',
        ordered: bull.length > 1
      });

      // Get each top-level item.
      cap = cap[0].match(this.rules.item);

      next = false;
      l = cap.length;
      i = 0;

      for (; i < l; i++) {
        item = cap[i];

        // Remove the list item's bullet
        // so it is seen as the next token.
        space = item.length;
        item = item.replace(/^ *([*+-]|\d+\.) +/, '');

        // Outdent whatever the
        // list item contains. Hacky.
        if (~item.indexOf('\n ')) {
          space -= item.length;
          item = !this.options.pedantic
            ? item.replace(new RegExp('^ {1,' + space + '}', 'gm'), '')
            : item.replace(/^ {1,4}/gm, '');
        }

        // Determine whether the next list item belongs here.
        // Backpedal if it does not belong in this list.
        if (this.options.smartLists && i !== l - 1) {
          b = block.bullet.exec(cap[i + 1])[0];
          if (bull !== b && !(bull.leng ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-markdown.marked.Parser"></a>[module gulp-markdown.marked.Parser](#apidoc.module.gulp-markdown.marked.Parser)

#### <a name="apidoc.element.gulp-markdown.marked.Parser.Parser"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Parser (options)](#apidoc.element.gulp-markdown.marked.Parser.Parser)
- description and source-code
```javascript
function Parser(options) {
  this.tokens = [];
  this.token = null;
  this.options = options || marked.defaults;
  this.options.renderer = this.options.renderer || new Renderer;
  this.renderer = this.options.renderer;
  this.renderer.options = this.options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Parser.parse"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.</span>parse (src, options, renderer)](#apidoc.element.gulp-markdown.marked.Parser.parse)
- description and source-code
```javascript
parse = function (src, options, renderer) {
  var parser = new Parser(options, renderer);
  return parser.parse(src);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-markdown.marked.Parser.prototype"></a>[module gulp-markdown.marked.Parser.prototype](#apidoc.module.gulp-markdown.marked.Parser.prototype)

#### <a name="apidoc.element.gulp-markdown.marked.Parser.prototype.next"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.prototype.</span>next ()](#apidoc.element.gulp-markdown.marked.Parser.prototype.next)
- description and source-code
```javascript
next = function () {
  return this.token = this.tokens.pop();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Parser.prototype.parse"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.prototype.</span>parse (src)](#apidoc.element.gulp-markdown.marked.Parser.prototype.parse)
- description and source-code
```javascript
parse = function (src) {
  this.inline = new InlineLexer(src.links, this.options, this.renderer);
  this.tokens = src.reverse();

  var out = '';
  while (this.next()) {
    out += this.tok();
  }

  return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Parser.prototype.parseText"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.prototype.</span>parseText ()](#apidoc.element.gulp-markdown.marked.Parser.prototype.parseText)
- description and source-code
```javascript
parseText = function () {
  var body = this.token.text;

  while (this.peek().type === 'text') {
    body += '\n' + this.next().text;
  }

  return this.inline.output(body);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Parser.prototype.peek"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.prototype.</span>peek ()](#apidoc.element.gulp-markdown.marked.Parser.prototype.peek)
- description and source-code
```javascript
peek = function () {
  return this.tokens[this.tokens.length - 1] || 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Parser.prototype.tok"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Parser.prototype.</span>tok ()](#apidoc.element.gulp-markdown.marked.Parser.prototype.tok)
- description and source-code
```javascript
tok = function () {
  switch (this.token.type) {
    case 'space': {
      return '';
    }
    case 'hr': {
      return this.renderer.hr();
    }
    case 'heading': {
      return this.renderer.heading(
        this.inline.output(this.token.text),
        this.token.depth,
        this.token.text);
    }
    case 'code': {
      return this.renderer.code(this.token.text,
        this.token.lang,
        this.token.escaped);
    }
    case 'table': {
      var header = ''
        , body = ''
        , i
        , row
        , cell
        , flags
        , j;

      // header
      cell = '';
      for (i = 0; i < this.token.header.length; i++) {
        flags = { header: true, align: this.token.align[i] };
        cell += this.renderer.tablecell(
          this.inline.output(this.token.header[i]),
          { header: true, align: this.token.align[i] }
        );
      }
      header += this.renderer.tablerow(cell);

      for (i = 0; i < this.token.cells.length; i++) {
        row = this.token.cells[i];

        cell = '';
        for (j = 0; j < row.length; j++) {
          cell += this.renderer.tablecell(
            this.inline.output(row[j]),
            { header: false, align: this.token.align[j] }
          );
        }

        body += this.renderer.tablerow(cell);
      }
      return this.renderer.table(header, body);
    }
    case 'blockquote_start': {
      var body = '';

      while (this.next().type !== 'blockquote_end') {
        body += this.tok();
      }

      return this.renderer.blockquote(body);
    }
    case 'list_start': {
      var body = ''
        , ordered = this.token.ordered;

      while (this.next().type !== 'list_end') {
        body += this.tok();
      }

      return this.renderer.list(body, ordered);
    }
    case 'list_item_start': {
      var body = '';

      while (this.next().type !== 'list_item_end') {
        body += this.token.type === 'text'
          ? this.parseText()
          : this.tok();
      }

      return this.renderer.listitem(body);
    }
    case 'loose_item_start': {
      var body = '';

      while (this.next().type !== 'list_item_end') {
        body += this.tok();
      }

      return this.renderer.listitem(body);
    }
    case 'html': {
      var html = !this.token.pre && !this.options.pedantic
        ? this.inline.output(this.token.text)
        : this.token.text;
      return this.renderer.html(html);
    }
    case 'paragraph': {
      return this.renderer.paragraph(this.inline.output(this.token.text));
    }
    case 'text': {
      return this.renderer.paragraph(this.parseText());
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-markdown.marked.Renderer"></a>[module gulp-markdown.marked.Renderer](#apidoc.module.gulp-markdown.marked.Renderer)

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.Renderer"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.</span>Renderer (options)](#apidoc.element.gulp-markdown.marked.Renderer.Renderer)
- description and source-code
```javascript
function Renderer(options) {
  this.options = options || {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-markdown.marked.Renderer.prototype"></a>[module gulp-markdown.marked.Renderer.prototype](#apidoc.module.gulp-markdown.marked.Renderer.prototype)

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.blockquote"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>blockquote (quote)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.blockquote)
- description and source-code
```javascript
blockquote = function (quote) {
  return '<blockquote>\n' + quote + '</blockquote>\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.br"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>br ()](#apidoc.element.gulp-markdown.marked.Renderer.prototype.br)
- description and source-code
```javascript
br = function () {
  return this.options.xhtml ? '<br/>' : '<br>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.code"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>code (code, lang, escaped)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.code)
- description and source-code
```javascript
code = function (code, lang, escaped) {
  if (this.options.highlight) {
    var out = this.options.highlight(code, lang);
    if (out != null && out !== code) {
      escaped = true;
      code = out;
    }
  }

  if (!lang) {
    return '<pre><code>'
      + (escaped ? code : escape(code, true))
      + '\n</code></pre>';
  }

  return '<pre><code class="'
    + this.options.langPrefix
    + escape(lang, true)
    + '">'
    + (escaped ? code : escape(code, true))
    + '\n</code></pre>\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.codespan"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>codespan (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.codespan)
- description and source-code
```javascript
codespan = function (text) {
  return '<code>' + text + '</code>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.del"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>del (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.del)
- description and source-code
```javascript
del = function (text) {
  return '<del>' + text + '</del>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.em"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>em (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.em)
- description and source-code
```javascript
em = function (text) {
  return '<em>' + text + '</em>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.heading"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>heading (text, level, raw)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.heading)
- description and source-code
```javascript
heading = function (text, level, raw) {
  return '<h'
    + level
    + ' id="'
    + this.options.headerPrefix
    + raw.toLowerCase().replace(/[^\w]+/g, '-')
    + '">'
    + text
    + '</h'
    + level
    + '>\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.hr"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>hr ()](#apidoc.element.gulp-markdown.marked.Renderer.prototype.hr)
- description and source-code
```javascript
hr = function () {
  return this.options.xhtml ? '<hr/>\n' : '<hr>\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.html"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>html (html)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.html)
- description and source-code
```javascript
html = function (html) {
  return html;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.image"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>image (href, title, text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.image)
- description and source-code
```javascript
image = function (href, title, text) {
  var out = '<img src="' + href + '" alt="' + text + '"';
  if (title) {
    out += ' title="' + title + '"';
  }
  out += this.options.xhtml ? '/>' : '>';
  return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.link"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>link (href, title, text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.link)
- description and source-code
```javascript
link = function (href, title, text) {
  if (this.options.sanitize) {
    try {
      var prot = decodeURIComponent(unescape(href))
        .replace(/[^\w:]/g, '')
        .toLowerCase();
    } catch (e) {
      return '';
    }
    if (prot.indexOf('javascript:') === 0 || prot.indexOf('vbscript:') === 0) {
      return '';
    }
  }
  var out = '<a href="' + href + '"';
  if (title) {
    out += ' title="' + title + '"';
  }
  out += '>' + text + '</a>';
  return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.list"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>list (body, ordered)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.list)
- description and source-code
```javascript
list = function (body, ordered) {
  var type = ordered ? 'ol' : 'ul';
  return '<' + type + '>\n' + body + '</' + type + '>\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.listitem"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>listitem (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.listitem)
- description and source-code
```javascript
listitem = function (text) {
  return '<li>' + text + '</li>\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.paragraph"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>paragraph (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.paragraph)
- description and source-code
```javascript
paragraph = function (text) {
  return '<p>' + text + '</p>\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.strong"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>strong (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.strong)
- description and source-code
```javascript
strong = function (text) {
  return '<strong>' + text + '</strong>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.table"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>table (header, body)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.table)
- description and source-code
```javascript
table = function (header, body) {
  return '<table>\n'
    + '<thead>\n'
    + header
    + '</thead>\n'
    + '<tbody>\n'
    + body
    + '</tbody>\n'
    + '</table>\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.tablecell"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>tablecell (content, flags)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.tablecell)
- description and source-code
```javascript
tablecell = function (content, flags) {
  var type = flags.header ? 'th' : 'td';
  var tag = flags.align
    ? '<' + type + ' style="text-align:' + flags.align + '">'
    : '<' + type + '>';
  return tag + content + '</' + type + '>\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.tablerow"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>tablerow (content)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.tablerow)
- description and source-code
```javascript
tablerow = function (content) {
  return '<tr>\n' + content + '</tr>\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-markdown.marked.Renderer.prototype.text"></a>[function <span class="apidocSignatureSpan">gulp-markdown.marked.Renderer.prototype.</span>text (text)](#apidoc.element.gulp-markdown.marked.Renderer.prototype.text)
- description and source-code
```javascript
text = function (text) {
  return text;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
