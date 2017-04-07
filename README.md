# api documentation for  [juice2 (v1.3.1)](https://github.com/andrewrk/juice)  [![npm package](https://img.shields.io/npm/v/npmdoc-juice2.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-juice2) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-juice2.svg)](https://travis-ci.org/npmdoc/node-npmdoc-juice2)
#### Inlines css into html source

[![NPM](https://nodei.co/npm/juice2.png?downloads=true)](https://www.npmjs.com/package/juice2)

[![apidoc](https://npmdoc.github.io/node-npmdoc-juice2/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-juice2_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-juice2/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-juice2/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-juice2/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bin": {
        "juice2": "./bin/juice"
    },
    "bugs": {
        "url": "https://github.com/andrewrk/juice/issues"
    },
    "dependencies": {
        "commander": "~2.3.0",
        "cssom": "~0.3.0",
        "jsdom": "~0.11.1",
        "pend": "~1.1.2",
        "slick": "~1.12.1",
        "superagent": "~0.18.2"
    },
    "description": "Inlines css into html source",
    "devDependencies": {
        "expresso": "~0.9.2",
        "mocha": "~1.20.1",
        "should": "~4.0.4"
    },
    "directories": {},
    "dist": {
        "shasum": "15c99929fdb49728a5b4fb41e9b1306739c19ec4",
        "tarball": "https://registry.npmjs.org/juice2/-/juice2-1.3.1.tgz"
    },
    "engines": {
        "node": ">=0.10.20"
    },
    "homepage": "https://github.com/andrewrk/juice",
    "maintainers": [
        {
            "name": "superjoe",
            "email": "superjoe30@gmail.com"
        },
        {
            "name": "jrit",
            "email": "jarrett@24m2.com"
        }
    ],
    "name": "juice2",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/andrewrk/juice.git"
    },
    "scripts": {
        "test": "mocha --reporter spec"
    },
    "version": "1.3.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module juice2](#apidoc.module.juice2)
1.  [function <span class="apidocSignatureSpan">juice2.</span>Property (prop, value, selector)](#apidoc.element.juice2.Property)
1.  [function <span class="apidocSignatureSpan">juice2.</span>Selector (text, spec)](#apidoc.element.juice2.Selector)
1.  [function <span class="apidocSignatureSpan">juice2.</span>inlineContent (html, css)](#apidoc.element.juice2.inlineContent)
1.  [function <span class="apidocSignatureSpan">juice2.</span>inlineDocument (document, css, options)](#apidoc.element.juice2.inlineDocument)
1.  [function <span class="apidocSignatureSpan">juice2.</span>juiceContent (html, options, callback)](#apidoc.element.juice2.juiceContent)
1.  [function <span class="apidocSignatureSpan">juice2.</span>juiceDocument (document, options, callback)](#apidoc.element.juice2.juiceDocument)
1.  [function <span class="apidocSignatureSpan">juice2.</span>juiceFile (filePath, options, callback)](#apidoc.element.juice2.juiceFile)
1.  object <span class="apidocSignatureSpan">juice2.</span>Property.prototype
1.  object <span class="apidocSignatureSpan">juice2.</span>Selector.prototype
1.  object <span class="apidocSignatureSpan">juice2.</span>ignoredPseudos
1.  object <span class="apidocSignatureSpan">juice2.</span>utils
1.  object <span class="apidocSignatureSpan">juice2.</span>widthElements
1.  string <span class="apidocSignatureSpan">juice2.</span>version

#### [module juice2.Property](#apidoc.module.juice2.Property)
1.  [function <span class="apidocSignatureSpan">juice2.</span>Property (prop, value, selector)](#apidoc.element.juice2.Property.Property)

#### [module juice2.Property.prototype](#apidoc.module.juice2.Property.prototype)
1.  [function <span class="apidocSignatureSpan">juice2.Property.prototype.</span>compare (property)](#apidoc.element.juice2.Property.prototype.compare)
1.  [function <span class="apidocSignatureSpan">juice2.Property.prototype.</span>toString ()](#apidoc.element.juice2.Property.prototype.toString)

#### [module juice2.Selector](#apidoc.module.juice2.Selector)
1.  [function <span class="apidocSignatureSpan">juice2.</span>Selector (text, spec)](#apidoc.element.juice2.Selector.Selector)

#### [module juice2.Selector.prototype](#apidoc.module.juice2.Selector.prototype)
1.  [function <span class="apidocSignatureSpan">juice2.Selector.prototype.</span>parsed ()](#apidoc.element.juice2.Selector.prototype.parsed)
1.  [function <span class="apidocSignatureSpan">juice2.Selector.prototype.</span>specificity ()](#apidoc.element.juice2.Selector.prototype.specificity)

#### [module juice2.utils](#apidoc.module.juice2.utils)
1.  [function <span class="apidocSignatureSpan">juice2.utils.</span>compare (a, b)](#apidoc.element.juice2.utils.compare)
1.  [function <span class="apidocSignatureSpan">juice2.utils.</span>extend (obj, src)](#apidoc.element.juice2.utils.extend)
1.  [function <span class="apidocSignatureSpan">juice2.utils.</span>extract (selectorText)](#apidoc.element.juice2.utils.extract)
1.  [function <span class="apidocSignatureSpan">juice2.utils.</span>getMediaQueryText ( css )](#apidoc.element.juice2.utils.getMediaQueryText)
1.  [function <span class="apidocSignatureSpan">juice2.utils.</span>jsdom (html)](#apidoc.element.juice2.utils.jsdom)
1.  [function <span class="apidocSignatureSpan">juice2.utils.</span>parseCSS (css)](#apidoc.element.juice2.utils.parseCSS)
1.  [function <span class="apidocSignatureSpan">juice2.utils.</span>toArray (arr)](#apidoc.element.juice2.utils.toArray)



# <a name="apidoc.module.juice2"></a>[module juice2](#apidoc.module.juice2)

#### <a name="apidoc.element.juice2.Property"></a>[function <span class="apidocSignatureSpan">juice2.</span>Property (prop, value, selector)](#apidoc.element.juice2.Property)
- description and source-code
```javascript
function Property(prop, value, selector) {
  this.prop = prop;
  this.value = value;
  this.selector = selector
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.juice2.Selector"></a>[function <span class="apidocSignatureSpan">juice2.</span>Selector (text, spec)](#apidoc.element.juice2.Selector)
- description and source-code
```javascript
function Selector(text, spec) {
  this.text = text;
  this.spec = spec;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.juice2.inlineContent"></a>[function <span class="apidocSignatureSpan">juice2.</span>inlineContent (html, css)](#apidoc.element.juice2.inlineContent)
- description and source-code
```javascript
function inlineContent(html, css) {
  var document = utils.jsdom(html);
  inlineDocument(document, css, {});
  var inner = document.innerHTML;
  // free the associated memory
  // with lazily created parentWindow
  try {
    document.parentWindow.close();
  } catch (cleanupErr) {}
  return inner;
}
```
- example usage
```shell
...
uses. Also be sure to clean up after you are done. You may have to
call 'document.parentWindow.close()' to free up memory.

 * 'document' - a jsdom instance
 * 'options' - see 'juice.juiceContent'
 * 'callback(err)'

### juice.inlineContent(html, css)

This takes html and css and returns new html with the provided css inlined.
It does not look at '<style>' or '<link rel="stylesheet">' elements at all.

### juice.inlineDocument(document, css, options)

Given a jsdom instance and css, this modifies the jsdom instance so that the
...
```

#### <a name="apidoc.element.juice2.inlineDocument"></a>[function <span class="apidocSignatureSpan">juice2.</span>inlineDocument (document, css, options)](#apidoc.element.juice2.inlineDocument)
- description and source-code
```javascript
function inlineDocument(document, css, options) {

  var rules = utils.parseCSS(css)
    , editedElements = [];

  rules.forEach(handleRule);
  editedElements.forEach(setStyleAttrs);

  if (options && options.applyWidthAttributes) {
    editedElements.forEach(setWidthAttrs);
  }

  function handleRule(rule) {
    var sel = rule[0]
      , style = rule[1]
      , selector = new Selector(sel);

    // skip rule if the selector has any pseudos which are ignored
    var parsedSelector = selector.parsed();
    for (var i = 0; i < parsedSelector.length; ++i) {
      var subSel = parsedSelector[i];
      if (subSel.pseudos) {
        for (var j = 0; j < subSel.pseudos.length; ++j) {
          var subSelPseudo = subSel.pseudos[j];
          if (juice.ignoredPseudos.indexOf(subSelPseudo.name) >= 0) return;
        }
      }
    }

    var els;
    try {
      els = document.querySelectorAll(sel);
    } catch (err) {
      // skip invalid selector
      return;
    }
    utils.toArray(els).forEach(function (el) {
      if (!el.styleProps) {
        el.styleProps = {}

        // if the element has inline styles, fake selector with topmost specificity
        if (el.getAttribute('style')) {
          var cssText = '* { ' + el.getAttribute('style') + ' } '
          addProps(utils.parseCSS(cssText)[0][1], styleSelector);
        }

        // store reference to an element we need to compile style="" attr for
        editedElements.push(el);
      }

      // go through the properties
      function addProps (style, selector) {
        for (var i = 0, l = style.length; i < l; i++) {
          var name = style[i]
            , value = style[name]
            , sel = style._importants[name] ? importantSelector : selector
            , prop = new Property(name, value, sel)
            , existing = el.styleProps[name];

          if (existing) {
            var winner = existing.compare(prop)
              , loser = prop === winner ? existing : prop

            if (winner === prop) el.styleProps[name] = prop;
          } else {
            el.styleProps[name] = prop;
          }
        }
      }

      addProps(style, selector);
    });
  }

  function setStyleAttrs(el) {
    var style = [];
    for (var i in el.styleProps) {
      style.push(el.styleProps[i].prop + ": " + el.styleProps[i].value.replace(/["]/g, "'") + ";");
    }
    // sorting will arrange styles like padding: before padding-bottom: which will preserve the expected styling
    style = style.sort( function ( a, b )
    {
      var aProp = a.split( ':' )[0];
      var bProp = b.split( ':' )[0];
      return ( aProp > bProp ? 1 : aProp < bProp ? -1 : 0 );
    } );
    el.setAttribute('style', style.join(' '));
  }

  function setWidthAttrs(el) {
    if (juice.widthElements.indexOf(el.nodeName) > -1) {
      for (var i in el.styleProps) {
        if (el.styleProps[i].prop === 'width' && el.styleProps[i].value.match(/px/)) {
          var pxWidth = el.styleProps[i].value.replace('px', '');
          el.setAttribute('width', pxWidth);
          return;
        }
      }
    }
  }
}
```
- example usage
```shell
...
 * 'callback(err)'

### juice.inlineContent(html, css)

This takes html and css and returns new html with the provided css inlined.
It does not look at '<style>' or '<link rel="stylesheet">' elements at all.

### juice.inlineDocument(document, css, options)

Given a jsdom instance and css, this modifies the jsdom instance so that the
provided css is inlined. It does not look at '<style>' or
'<link rel="stylesheet">' elements at all.

### juice.ignoredPseudos
...
```

#### <a name="apidoc.element.juice2.juiceContent"></a>[function <span class="apidocSignatureSpan">juice2.</span>juiceContent (html, options, callback)](#apidoc.element.juice2.juiceContent)
- description and source-code
```javascript
function juiceContent(html, options, callback) {
  assert.ok(options.url, "options.url is required");
  options = getDefaultOptions(options);
  // hack to force jsdom to see this argument as html content, not a url
  // or a filename. https://github.com/tmpvar/jsdom/issues/554
  html += "\n";
  var document = utils.jsdom(html);
  juiceDocument(document, options, function(err) {
    if (err) {
      // free the associated memory
      // with lazily created parentWindow
      try {
       document.parentWindow.close();
      } catch (cleanupErr) {}
      callback(err);
    } else {
      var inner = document.innerHTML;
      // free the associated memory
      // with lazily created parentWindow
      try {
        document.parentWindow.close();
      } catch (cleanupErr) {}
      callback(null, inner);
    }
  });
}
```
- example usage
```shell
...
     to override, be sure your 'url' has the protocol at the beginning, e.g.
     'http://' or 'file://'.
 * 'callback(err, html)'
   - 'err' - 'Error' object or 'null'.
   - 'html' - contains the html from 'filePath', with potentially '<style>' and
     '<link rel="stylesheet">' tags removed, and css inlined.

### juice.juiceContent(html, options, callback)

 * 'html' - raw html content
 * 'options' - same options as calling 'juice', except now 'url' is required.
 * 'callback(err, html)' - same as calling 'juice'

### juice.juiceDocument(document, options, callback)
...
```

#### <a name="apidoc.element.juice2.juiceDocument"></a>[function <span class="apidocSignatureSpan">juice2.</span>juiceDocument (document, options, callback)](#apidoc.element.juice2.juiceDocument)
- description and source-code
```javascript
function juiceDocument(document, options, callback) {
  assert.ok(options.url, "options.url is required");
  options = getDefaultOptions(options);
  extractCssFromDocument(document, options, function(err, css) {
    css += "\n" + options.extraCss;
    inlineDocumentWithCb(document, css, options, callback);
  });
}
```
- example usage
```shell
...

### juice.juiceContent(html, options, callback)

* 'html' - raw html content
* 'options' - same options as calling 'juice', except now 'url' is required.
* 'callback(err, html)' - same as calling 'juice'

### juice.juiceDocument(document, options, callback)

Operates on a jsdom instance. Be sure to use the same jsdom version that juice
uses. Also be sure to clean up after you are done. You may have to
call 'document.parentWindow.close()' to free up memory.

* 'document' - a jsdom instance
* 'options' - see 'juice.juiceContent'
...
```

#### <a name="apidoc.element.juice2.juiceFile"></a>[function <span class="apidocSignatureSpan">juice2.</span>juiceFile (filePath, options, callback)](#apidoc.element.juice2.juiceFile)
- description and source-code
```javascript
function juiceFile(filePath, options, callback) {
  // set default options
  fs.readFile(filePath, 'utf8', function(err, content) {
    if (err) return callback(err);
    options = getDefaultOptions(options); // so we can mutate options without guilt
    var slashes = os.platform() === 'win32' ? '\\\\' : '//';
    options.url = options.url || ("file:" + slashes + path.resolve(process.cwd(), filePath));
    juiceContent(content, options, callback);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.juice2.Property"></a>[module juice2.Property](#apidoc.module.juice2.Property)

#### <a name="apidoc.element.juice2.Property.Property"></a>[function <span class="apidocSignatureSpan">juice2.</span>Property (prop, value, selector)](#apidoc.element.juice2.Property.Property)
- description and source-code
```javascript
function Property(prop, value, selector) {
  this.prop = prop;
  this.value = value;
  this.selector = selector
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.juice2.Property.prototype"></a>[module juice2.Property.prototype](#apidoc.module.juice2.Property.prototype)

#### <a name="apidoc.element.juice2.Property.prototype.compare"></a>[function <span class="apidocSignatureSpan">juice2.Property.prototype.</span>compare (property)](#apidoc.element.juice2.Property.prototype.compare)
- description and source-code
```javascript
compare = function (property) {
  var a = this.selector.specificity()
    , b = property.selector.specificity()
    , winner = compare(a, b)

  if (winner == a) return this;
  return property;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.juice2.Property.prototype.toString"></a>[function <span class="apidocSignatureSpan">juice2.Property.prototype.</span>toString ()](#apidoc.element.juice2.Property.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.prop + ': ' + this.value.replace(/['"]+/g, '') + ';';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.juice2.Selector"></a>[module juice2.Selector](#apidoc.module.juice2.Selector)

#### <a name="apidoc.element.juice2.Selector.Selector"></a>[function <span class="apidocSignatureSpan">juice2.</span>Selector (text, spec)](#apidoc.element.juice2.Selector.Selector)
- description and source-code
```javascript
function Selector(text, spec) {
  this.text = text;
  this.spec = spec;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.juice2.Selector.prototype"></a>[module juice2.Selector.prototype](#apidoc.module.juice2.Selector.prototype)

#### <a name="apidoc.element.juice2.Selector.prototype.parsed"></a>[function <span class="apidocSignatureSpan">juice2.Selector.prototype.</span>parsed ()](#apidoc.element.juice2.Selector.prototype.parsed)
- description and source-code
```javascript
parsed = function () {
  if (!this.tokens) this.tokens = parse(this.text);
  return this.tokens;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.juice2.Selector.prototype.specificity"></a>[function <span class="apidocSignatureSpan">juice2.Selector.prototype.</span>specificity ()](#apidoc.element.juice2.Selector.prototype.specificity)
- description and source-code
```javascript
specificity = function () {
  if (!this.spec) this.spec = specificity(this.text, this.parsed());
  return this.spec;

  function specificity (text, parsed) {
    var expressions = parsed || parse(text)
      , spec = [0, 0, 0, 0]
      , nots = []

    for (var i = 0; i < expressions.length; i++) {
      var expression = expressions[i]
        , pseudos = expression.pseudos

      // id awards a point in the second column
      if (expression.id) spec[1]++;

      // classes and attributes award a point each in the third column
      if (expression.attributes) spec[2] += expression.attributes.length;
      if (expression.classList) spec[2] += expression.classList.length;

      // tag awards a point in the fourth column
      if (expression.tag && expression.tag !== '*') spec[3]++;

      // pseudos award a point each in the fourth column
      if (pseudos) {
        spec[3] += pseudos.length;

        for (var p = 0; p < pseudos.length; p++) {
         if (pseudos[p].key === 'not'){
            nots.push(pseudos[p].value);
            spec[3]--;
          }
        }
      }
    }

    for (var ii = nots.length; ii--;) {
      var not = specificity(nots[ii]);
      for (var jj = 4; jj--;) spec[jj] += not[jj];
    }

    return spec;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.juice2.utils"></a>[module juice2.utils](#apidoc.module.juice2.utils)

#### <a name="apidoc.element.juice2.utils.compare"></a>[function <span class="apidocSignatureSpan">juice2.utils.</span>compare (a, b)](#apidoc.element.juice2.utils.compare)
- description and source-code
```javascript
compare = function (a, b) {
  for (var i = 0; i < 4; i++) {
    if (a[i] === b[i]) continue;
    if (a[i] > b[i]) return a;
    return b;
  }

  return b;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.juice2.utils.extend"></a>[function <span class="apidocSignatureSpan">juice2.utils.</span>extend (obj, src)](#apidoc.element.juice2.utils.extend)
- description and source-code
```javascript
extend = function (obj, src) {
  for (var key in src) if (own.call(src, key)) obj[key] = src[key];
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.juice2.utils.extract"></a>[function <span class="apidocSignatureSpan">juice2.utils.</span>extract (selectorText)](#apidoc.element.juice2.utils.extract)
- description and source-code
```javascript
function extract(selectorText) {
  var attr = 0
    , sels = []
    , sel = ''

  for (var i = 0, l = selectorText.length; i < l; i++) {
    var c = selectorText.charAt(i);

    if (attr) {
      if (']' === c || ')' === c) attr--;
      sel += c;
    } else {
      if (',' === c) {
        sels.push(sel);
        sel = '';
      } else {
        if ('[' === c || '(' === c) attr++;
        if (sel.length || (c !== ',' && c !== '\n' && c !== ' ')) sel += c;
      }
    }
  }

  if (sel.length) sels.push(sel);

  return sels;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.juice2.utils.getMediaQueryText"></a>[function <span class="apidocSignatureSpan">juice2.utils.</span>getMediaQueryText ( css )](#apidoc.element.juice2.utils.getMediaQueryText)
- description and source-code
```javascript
getMediaQueryText = function ( css )
{
	var rules = cssom.parse( css ).cssRules || []
	var queries = [];

	for ( var i = 0, l = rules.length; i < l; i++ )
	{
		/* CSS types
		  STYLE: 1,
		  IMPORT: 3,
		  MEDIA: 4,
		  FONT_FACE: 5,
		 */

		if ( rules[i].type === cssom.CSSMediaRule.prototype.type )
		{
			var query = rules[i];
			var queryString = [];

			queryString.push( os.EOL + "@media " + query.media[0] + " {" );

			for ( var ii = 0, ll = query.cssRules.length; ii < ll; ii++ )
			{
				var rule = query.cssRules[ii];

				if ( rule.type === cssom.CSSStyleRule.prototype.type || rule.type === cssom.CSSFontFaceRule.prototype.type )
				{
					queryString.push( "  " + ( rule.type === cssom.CSSStyleRule.prototype.type ? rule.selectorText : "@font-face" ) + " {" );

					for ( var style = 0; style < rule.style.length; style++ )
					{
						var property = rule.style[style];
						var value = rule.style[property];
						var important = rule.style._importants[property] ? " !important" : "";
						queryString.push( "    " + property + ": " + value + important + ";" );
					}
					queryString.push( "  }" );
				}
			}

			queryString.push( "}" );
			var result = queryString.length ? queryString.join( os.EOL ) + os.EOL : "";

			queries.push( result );
		}
	}

	return queries.join( os.EOL );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.juice2.utils.jsdom"></a>[function <span class="apidocSignatureSpan">juice2.utils.</span>jsdom (html)](#apidoc.element.juice2.utils.jsdom)
- description and source-code
```javascript
jsdom = function (html) {
  return jsdom.html(html, null, {
    features: {
        QuerySelector: ['1.0']
      , FetchExternalResources: false
      , ProcessExternalResources: false
      , MutationEvents: false
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.juice2.utils.parseCSS"></a>[function <span class="apidocSignatureSpan">juice2.utils.</span>parseCSS (css)](#apidoc.element.juice2.utils.parseCSS)
- description and source-code
```javascript
parseCSS = function (css) {
  var rules = cssom.parse(css).cssRules || []
    , ret = []

  for (var i = 0, l = rules.length; i < l; i++) {
    if (rules[i].selectorText) { // media queries don't have selectorText
      var rule = rules[i]
        , selectors = exports.extract(rule.selectorText)

      for (var ii = 0, ll = selectors.length; ii < ll; ii++) {
        ret.push([selectors[ii], rule.style]);
      }
    }
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.juice2.utils.toArray"></a>[function <span class="apidocSignatureSpan">juice2.utils.</span>toArray (arr)](#apidoc.element.juice2.utils.toArray)
- description and source-code
```javascript
toArray = function (arr) {
  var ret = [];

  for (var i = 0, l = arr.length; i < l; i++)
    ret.push(arr[i]);

  return ret;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
