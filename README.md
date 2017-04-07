# api documentation for  [papaparse (v4.2.0)](http://papaparse.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-papaparse.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-papaparse) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-papaparse.svg)](https://travis-ci.org/npmdoc/node-npmdoc-papaparse)
#### Fast and powerful CSV parser for the browser that supports web workers and streaming large files. Converts CSV to JSON and JSON to CSV.

[![NPM](https://nodei.co/npm/papaparse.png?downloads=true)](https://www.npmjs.com/package/papaparse)

[![apidoc](https://npmdoc.github.io/node-npmdoc-papaparse/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-papaparse_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-papaparse/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-papaparse/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-papaparse/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matthew Holt",
        "url": "https://twitter.com/mholt6"
    },
    "bugs": {
        "url": "https://github.com/mholt/PapaParse/issues"
    },
    "dependencies": {},
    "description": "Fast and powerful CSV parser for the browser that supports web workers and streaming large files. Converts CSV to JSON and JSON to CSV.",
    "devDependencies": {
        "chai": "^3.0.0",
        "connect": "^3.3.3",
        "grunt": "^0.4.5",
        "grunt-contrib-uglify": "^0.6.0",
        "mocha": "^2.2.5",
        "mocha-phantomjs": "^3.5.4",
        "open": "0.0.5",
        "phantomjs": "1.9.1 - 1.9.7-15",
        "serve-static": "^1.7.1"
    },
    "directories": {},
    "dist": {
        "shasum": "ac5bed7de39445dabb6616a507024b8b88eee7c3",
        "tarball": "https://registry.npmjs.org/papaparse/-/papaparse-4.2.0.tgz"
    },
    "gitHead": "fd6431e385468ef3c1c64f7ccb4c47c435631e25",
    "homepage": "http://papaparse.com",
    "keywords": [
        "csv",
        "parser",
        "parse",
        "parsing",
        "delimited",
        "text",
        "data",
        "auto-detect",
        "comma",
        "tab",
        "pipe",
        "file",
        "filereader",
        "stream",
        "worker",
        "workers",
        "thread",
        "threading",
        "multi-threaded",
        "jquery-plugin"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "http://opensource.org/licenses/MIT"
        }
    ],
    "main": "papaparse.js",
    "maintainers": [
        {
            "name": "mholt",
            "email": "Matthew.Holt+npm@gmail.com"
        },
        {
            "name": "pokoli",
            "email": "sergi@koolpi.com"
        }
    ],
    "name": "papaparse",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mholt/PapaParse.git"
    },
    "scripts": {
        "test": "npm run test-node && npm run test-phantomjs",
        "test-browser": "node tests/test.js",
        "test-node": "mocha tests/node-tests.js tests/test-cases.js",
        "test-phantomjs": "node tests/test.js --phantomjs"
    },
    "version": "4.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module papaparse](#apidoc.module.papaparse)
1.  boolean <span class="apidocSignatureSpan">papaparse.</span>WORKERS_SUPPORTED
1.  [function <span class="apidocSignatureSpan">papaparse.</span>FileStreamer (config)](#apidoc.element.papaparse.FileStreamer)
1.  [function <span class="apidocSignatureSpan">papaparse.</span>NetworkStreamer (config)](#apidoc.element.papaparse.NetworkStreamer)
1.  [function <span class="apidocSignatureSpan">papaparse.</span>Parser (config)](#apidoc.element.papaparse.Parser)
1.  [function <span class="apidocSignatureSpan">papaparse.</span>ParserHandle (_config)](#apidoc.element.papaparse.ParserHandle)
1.  [function <span class="apidocSignatureSpan">papaparse.</span>ReadableStreamStreamer (config)](#apidoc.element.papaparse.ReadableStreamStreamer)
1.  [function <span class="apidocSignatureSpan">papaparse.</span>StringStreamer (config)](#apidoc.element.papaparse.StringStreamer)
1.  [function <span class="apidocSignatureSpan">papaparse.</span>parse (_input, _config)](#apidoc.element.papaparse.parse)
1.  [function <span class="apidocSignatureSpan">papaparse.</span>unparse (_input, _config)](#apidoc.element.papaparse.unparse)
1.  number <span class="apidocSignatureSpan">papaparse.</span>LocalChunkSize
1.  number <span class="apidocSignatureSpan">papaparse.</span>RemoteChunkSize
1.  object <span class="apidocSignatureSpan">papaparse.</span>BAD_DELIMITERS
1.  object <span class="apidocSignatureSpan">papaparse.</span>FileStreamer.prototype
1.  object <span class="apidocSignatureSpan">papaparse.</span>NetworkStreamer.prototype
1.  object <span class="apidocSignatureSpan">papaparse.</span>ReadableStreamStreamer.prototype
1.  object <span class="apidocSignatureSpan">papaparse.</span>SCRIPT_PATH
1.  object <span class="apidocSignatureSpan">papaparse.</span>StringStreamer.prototype
1.  string <span class="apidocSignatureSpan">papaparse.</span>BYTE_ORDER_MARK
1.  string <span class="apidocSignatureSpan">papaparse.</span>DefaultDelimiter
1.  string <span class="apidocSignatureSpan">papaparse.</span>RECORD_SEP
1.  string <span class="apidocSignatureSpan">papaparse.</span>UNIT_SEP

#### [module papaparse.FileStreamer](#apidoc.module.papaparse.FileStreamer)
1.  [function <span class="apidocSignatureSpan">papaparse.</span>FileStreamer (config)](#apidoc.element.papaparse.FileStreamer.FileStreamer)

#### [module papaparse.FileStreamer.prototype](#apidoc.module.papaparse.FileStreamer.prototype)
1.  [function <span class="apidocSignatureSpan">papaparse.FileStreamer.prototype.</span>constructor (config)](#apidoc.element.papaparse.FileStreamer.prototype.constructor)

#### [module papaparse.NetworkStreamer](#apidoc.module.papaparse.NetworkStreamer)
1.  [function <span class="apidocSignatureSpan">papaparse.</span>NetworkStreamer (config)](#apidoc.element.papaparse.NetworkStreamer.NetworkStreamer)

#### [module papaparse.NetworkStreamer.prototype](#apidoc.module.papaparse.NetworkStreamer.prototype)
1.  [function <span class="apidocSignatureSpan">papaparse.NetworkStreamer.prototype.</span>constructor (config)](#apidoc.element.papaparse.NetworkStreamer.prototype.constructor)

#### [module papaparse.ReadableStreamStreamer](#apidoc.module.papaparse.ReadableStreamStreamer)
1.  [function <span class="apidocSignatureSpan">papaparse.</span>ReadableStreamStreamer (config)](#apidoc.element.papaparse.ReadableStreamStreamer.ReadableStreamStreamer)

#### [module papaparse.ReadableStreamStreamer.prototype](#apidoc.module.papaparse.ReadableStreamStreamer.prototype)
1.  [function <span class="apidocSignatureSpan">papaparse.ReadableStreamStreamer.prototype.</span>constructor (config)](#apidoc.element.papaparse.ReadableStreamStreamer.prototype.constructor)

#### [module papaparse.StringStreamer](#apidoc.module.papaparse.StringStreamer)
1.  [function <span class="apidocSignatureSpan">papaparse.</span>StringStreamer (config)](#apidoc.element.papaparse.StringStreamer.StringStreamer)

#### [module papaparse.StringStreamer.prototype](#apidoc.module.papaparse.StringStreamer.prototype)
1.  [function <span class="apidocSignatureSpan">papaparse.StringStreamer.prototype.</span>constructor (config)](#apidoc.element.papaparse.StringStreamer.prototype.constructor)



# <a name="apidoc.module.papaparse"></a>[module papaparse](#apidoc.module.papaparse)

#### <a name="apidoc.element.papaparse.FileStreamer"></a>[function <span class="apidocSignatureSpan">papaparse.</span>FileStreamer (config)](#apidoc.element.papaparse.FileStreamer)
- description and source-code
```javascript
function FileStreamer(config)
	{
		config = config || {};
		if (!config.chunkSize)
			config.chunkSize = Papa.LocalChunkSize;
		ChunkStreamer.call(this, config);

		var reader, slice;

		// FileReader is better than FileReaderSync (even in worker) - see http://stackoverflow.com/q/24708649/1048862
		// But Firefox is a pill, too - see issue #76: https://github.com/mholt/PapaParse/issues/76
		var usingAsyncReader = typeof FileReader !== 'undefined';	// Safari doesn't consider it a function - see issue #105

		this.stream = function(file)
		{
			this._input = file;
			slice = file.slice || file.webkitSlice || file.mozSlice;

			if (usingAsyncReader)
			{
				reader = new FileReader();		// Preferred method of reading files, even in workers
				reader.onload = bindFunction(this._chunkLoaded, this);
				reader.onerror = bindFunction(this._chunkError, this);
			}
			else
				reader = new FileReaderSync();	// Hack for running in a web worker in Firefox

			this._nextChunk();	// Starts streaming
		};

		this._nextChunk = function()
		{
			if (!this._finished && (!this._config.preview || this._rowCount < this._config.preview))
				this._readChunk();
		}

		this._readChunk = function()
		{
			var input = this._input;
			if (this._config.chunkSize)
			{
				var end = Math.min(this._start + this._config.chunkSize, this._input.size);
				input = slice.call(input, this._start, end);
			}
			var txt = reader.readAsText(input, this._config.encoding);
			if (!usingAsyncReader)
				this._chunkLoaded({ target: { result: txt } });	// mimic the async signature
		}

		this._chunkLoaded = function(event)
		{
			// Very important to increment start each time before handling results
			this._start += this._config.chunkSize;
			this._finished = !this._config.chunkSize || this._start >= this._input.size;
			this.parseChunk(event.target.result);
		}

		this._chunkError = function()
		{
			this._sendError(reader.error);
		}

	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.papaparse.NetworkStreamer"></a>[function <span class="apidocSignatureSpan">papaparse.</span>NetworkStreamer (config)](#apidoc.element.papaparse.NetworkStreamer)
- description and source-code
```javascript
function NetworkStreamer(config)
	{
		config = config || {};
		if (!config.chunkSize)
			config.chunkSize = Papa.RemoteChunkSize;
		ChunkStreamer.call(this, config);

		var xhr;

		if (IS_WORKER)
		{
			this._nextChunk = function()
			{
				this._readChunk();
				this._chunkLoaded();
			};
		}
		else
		{
			this._nextChunk = function()
			{
				this._readChunk();
			};
		}

		this.stream = function(url)
		{
			this._input = url;
			this._nextChunk();	// Starts streaming
		};

		this._readChunk = function()
		{
			if (this._finished)
			{
				this._chunkLoaded();
				return;
			}

			xhr = new XMLHttpRequest();

			if (this._config.withCredentials)
			{
				xhr.withCredentials = this._config.withCredentials;
			}

			if (!IS_WORKER)
			{
				xhr.onload = bindFunction(this._chunkLoaded, this);
				xhr.onerror = bindFunction(this._chunkError, this);
			}

			xhr.open('GET', this._input, !IS_WORKER);

			if (this._config.chunkSize)
			{
				var end = this._start + this._config.chunkSize - 1;	// minus one because byte range is inclusive
				xhr.setRequestHeader('Range', 'bytes='+this._start+'-'+end);
				xhr.setRequestHeader('If-None-Match', 'webkit-no-cache'); // https://bugs.webkit.org/show_bug.cgi?id=82672
			}

			try {
				xhr.send();
			}
			catch (err) {
				this._chunkError(err.message);
			}

			if (IS_WORKER && xhr.status === 0)
				this._chunkError();
			else
				this._start += this._config.chunkSize;
		}

		this._chunkLoaded = function()
		{
			if (xhr.readyState != 4)
				return;

			if (xhr.status < 200 || xhr.status >= 400)
			{
				this._chunkError();
				return;
			}

			this._finished = !this._config.chunkSize || this._start > getFileSize(xhr);
			this.parseChunk(xhr.responseText);
		}

		this._chunkError = function(errorMessage)
		{
			var errorText = xhr.statusText || errorMessage;
			this._sendError(errorText);
		}

		function getFileSize(xhr)
		{
			var contentRange = xhr.getResponseHeader('Content-Range');
			if (contentRange === null) { // no content range, then finish!
        			return -1;
            		}
			return parseInt(contentRange.substr(contentRange.lastIndexOf('/') + 1));
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.papaparse.Parser"></a>[function <span class="apidocSignatureSpan">papaparse.</span>Parser (config)](#apidoc.element.papaparse.Parser)
- description and source-code
```javascript
function Parser(config)
	{
		// Unpack the config object
		config = config || {};
		var delim = config.delimiter;
		var newline = config.newline;
		var comments = config.comments;
		var step = config.step;
		var preview = config.preview;
		var fastMode = config.fastMode;
		var quoteChar = config.quoteChar || '"';

		// Delimiter must be valid
		if (typeof delim !== 'string'
			|| Papa.BAD_DELIMITERS.indexOf(delim) > -1)
			delim = ',';

		// Comment character must be valid
		if (comments === delim)
			throw 'Comment character same as delimiter';
		else if (comments === true)
			comments = '#';
		else if (typeof comments !== 'string'
			|| Papa.BAD_DELIMITERS.indexOf(comments) > -1)
			comments = false;

		// Newline must be valid: \r, \n, or \r\n
		if (newline != '\n' && newline != '\r' && newline != '\r\n')
			newline = '\n';

		// We're gonna need these at the Parser scope
		var cursor = 0;
		var aborted = false;

		this.parse = function(input, baseIndex, ignoreLastRow)
		{
			// For some reason, in Chrome, this speeds things up (!?)
			if (typeof input !== 'string')
				throw 'Input must be a string';

			// We don't need to compute some of these every time parse() is called,
			// but having them in a more local scope seems to perform better
			var inputLen = input.length,
				delimLen = delim.length,
				newlineLen = newline.length,
				commentsLen = comments.length;
			var stepIsFunction = typeof step === 'function';

			// Establish starting state
			cursor = 0;
			var data = [], errors = [], row = [], lastCursor = 0;

			if (!input)
				return returnable();

			if (fastMode || (fastMode !== false && input.indexOf(quoteChar) === -1))
			{
				var rows = input.split(newline);
				for (var i = 0; i < rows.length; i++)
				{
					var row = rows[i];
					cursor += row.length;
					if (i !== rows.length - 1)
						cursor += newline.length;
					else if (ignoreLastRow)
						return returnable();
					if (comments && row.substr(0, commentsLen) === comments)
						continue;
					if (stepIsFunction)
					{
						data = [];
						pushRow(row.split(delim));
						doStep();
						if (aborted)
							return returnable();
					}
					else
						pushRow(row.split(delim));
					if (preview && i >= preview)
					{
						data = data.slice(0, preview);
						return returnable(true);
					}
				}
				return returnable();
			}

			var nextDelim = input.indexOf(delim, cursor);
			var nextNewline = input.indexOf(newline, cursor);
			var quoteCharRegex = new RegExp(quoteChar+quoteChar, 'g');

			// Parser loop
			for (;;)
			{
				// Field has opening quote
				if (input[cursor] === quoteChar)
				{
					// Start our search for the closing quote where the cursor is
					var quoteSearch = cursor;

					// Skip the opening quote
					cursor++;

					for (;;)
					{
						// Find closing quote
						var quoteSearch = input.indexOf(quoteChar, quoteSearch+1);

						if (quoteSearch === -1)
						{
							if (!ignoreLastRow) {
								// No closing quote... what a pity
								errors.push({
									type: 'Quotes',
									code: 'MissingQuotes',
									message: 'Quoted field unterminated',
									row: data.length,	// row has yet to be inserted
									index: cursor
								});
							}
							return finish();
						}

						if (quoteSearch === inputLen-1)
						{
							// Closing quote at EOF
							var value = input.substring(cursor, quoteSearch).replace(quoteCharRegex, quoteChar);
							return finish(value);
						}

						// If this quote is escaped, it's part of the data; skip it
						if (input[quoteSearch+1] === quoteChar)
						{
							quoteSearch++;
							continue;
						}

						if (input[quoteSearch+1] === delim)
						{
							// Closing quote followed by delimiter
							row.push(input.substring(cursor, quoteSearch).replace(quoteCharRegex, quoteChar));
							cursor = quoteSearch + 1 + delimLen;
							nextDelim = input.indexOf(delim, cursor);
							nextNewline = input.indexOf(newline, cursor);
							break;
						}

						if (input.substr(quoteSearch+1, newlineLen) === newline)
						{
							// Closing quote followed b ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.papaparse.ParserHandle"></a>[function <span class="apidocSignatureSpan">papaparse.</span>ParserHandle (_config)](#apidoc.element.papaparse.ParserHandle)
- description and source-code
```javascript
function ParserHandle(_config)
	{
		// One goal is to minimize the use of regular expressions...
		var FLOAT = /^\s*-?(\d*\.?\d+|\d+\.?\d*)(e[-+]?\d+)?\s*$/i;

		var self = this;
		var _stepCounter = 0;	// Number of times step was called (number of rows parsed)
		var _input;				// The input being parsed
		var _parser;			// The core parser being used
		var _paused = false;	// Whether we are paused or not
		var _aborted = false;   // Whether the parser has aborted or not
		var _delimiterError;	// Temporary state between delimiter detection and processing results
		var _fields = [];		// Fields are from the header row of the input, if there is one
		var _results = {		// The last results returned from the parser
			data: [],
			errors: [],
			meta: {}
		};

		if (isFunction(_config.step))
		{
			var userStep = _config.step;
			_config.step = function(results)
			{
				_results = results;

				if (needsHeaderRow())
					processResults();
				else	// only call user's step function after header row
				{
					processResults();

					// It's possbile that this line was empty and there's no row here after all
					if (_results.data.length === 0)
						return;

					_stepCounter += results.data.length;
					if (_config.preview && _stepCounter > _config.preview)
						_parser.abort();
					else
						userStep(_results, self);
				}
			};
		}

		<span class="apidocCodeCommentSpan">/**
		 * Parses input. Most users won't need, and shouldn't mess with, the baseIndex
		 * and ignoreLastRow parameters. They are used by streamers (wrapper functions)
		 * when an input comes in multiple chunks, like from a file.
		 */
</span>		this.parse = function(input, baseIndex, ignoreLastRow)
		{
			if (!_config.newline)
				_config.newline = guessLineEndings(input);

			_delimiterError = false;
			if (!_config.delimiter)
			{
				var delimGuess = guessDelimiter(input, _config.newline);
				if (delimGuess.successful)
					_config.delimiter = delimGuess.bestDelimiter;
				else
				{
					_delimiterError = true;	// add error after parsing (otherwise it would be overwritten)
					_config.delimiter = Papa.DefaultDelimiter;
				}
				_results.meta.delimiter = _config.delimiter;
			}
			else if(typeof _config.delimiter === 'function')
			{
				_config.delimiter = _config.delimiter(input);
				_results.meta.delimiter = _config.delimiter;
			}

			var parserConfig = copy(_config);
			if (_config.preview && _config.header)
				parserConfig.preview++;	// to compensate for header row

			_input = input;
			_parser = new Parser(parserConfig);
			_results = _parser.parse(_input, baseIndex, ignoreLastRow);
			processResults();
			return _paused ? { meta: { paused: true } } : (_results || { meta: { paused: false } });
		};

		this.paused = function()
		{
			return _paused;
		};

		this.pause = function()
		{
			_paused = true;
			_parser.abort();
			_input = _input.substr(_parser.getCharIndex());
		};

		this.resume = function()
		{
			_paused = false;
			self.streamer.parseChunk(_input);
		};

		this.aborted = function ()
		{
			return _aborted;
		};

		this.abort = function()
		{
			_aborted = true;
			_parser.abort();
			_results.meta.aborted = true;
			if (isFunction(_config.complete))
				_config.complete(_results);
			_input = '';
		};

		function processResults()
		{
			if (_results && _delimiterError)
			{
				addError('Delimiter', 'UndetectableDelimiter', 'Unable to auto-detect delimiting character; defaulted to \''+Papa.DefaultDelimiter
+'\'');
				_delimiterError = false;
			}

			if (_config.skipEmptyLines)
			{
				for (var i = 0; i < _results.data.length; i++)
					if (_results.data[i].length === 1 && _results.data[i][0] === '')
						_results.data.splice(i--, 1);
			}

			if (needsHeaderRow())
				fillHeaderFields();

			return applyHeaderAndDynamicTyping();
		}

		function needsHeaderRow()
		{
			return _config.header && _fields.length === 0;
		}

		function fillHeaderFields()
		{
			if (!_results)
				return;
			for (var i = 0; needsHeaderRow() && i < _results.data.length; i++)
				for (var j = 0; j < _results.data[i].length; j++)
					_fields.push(_results.data[i][j]);
			_results.data.spli ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.papaparse.ReadableStreamStreamer"></a>[function <span class="apidocSignatureSpan">papaparse.</span>ReadableStreamStreamer (config)](#apidoc.element.papaparse.ReadableStreamStreamer)
- description and source-code
```javascript
function ReadableStreamStreamer(config)
	{
		config = config || {};

		ChunkStreamer.call(this, config);

		var queue = [];
		var parseOnData = true;

		this.stream = function(stream)
		{
			this._input = stream;

			this._input.on('data', this._streamData);
			this._input.on('end', this._streamEnd);
			this._input.on('error', this._streamError);
		}

		this._nextChunk = function()
		{
			if (queue.length)
			{
				this.parseChunk(queue.shift());
			}
			else
			{
				parseOnData = true;
			}
		}

		this._streamData = bindFunction(function(chunk)
		{
			try
			{
				queue.push(typeof chunk === 'string' ? chunk : chunk.toString(this._config.encoding));

				if (parseOnData)
				{
					parseOnData = false;
					this.parseChunk(queue.shift());
				}
			}
			catch (error)
			{
				this._streamError(error);
			}
		}, this);

		this._streamError = bindFunction(function(error)
		{
			this._streamCleanUp();
			this._sendError(error.message);
		}, this);

		this._streamEnd = bindFunction(function()
		{
			this._streamCleanUp();
			this._finished = true;
			this._streamData('');
		}, this);

		this._streamCleanUp = bindFunction(function()
		{
			this._input.removeListener('data', this._streamData);
			this._input.removeListener('end', this._streamEnd);
			this._input.removeListener('error', this._streamError);
		}, this);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.papaparse.StringStreamer"></a>[function <span class="apidocSignatureSpan">papaparse.</span>StringStreamer (config)](#apidoc.element.papaparse.StringStreamer)
- description and source-code
```javascript
function StringStreamer(config)
	{
		config = config || {};
		ChunkStreamer.call(this, config);

		var string;
		var remaining;
		this.stream = function(s)
		{
			string = s;
			remaining = s;
			return this._nextChunk();
		}
		this._nextChunk = function()
		{
			if (this._finished) return;
			var size = this._config.chunkSize;
			var chunk = size ? remaining.substr(0, size) : remaining;
			remaining = size ? remaining.substr(size) : '';
			this._finished = !remaining;
			return this.parseChunk(chunk);
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.papaparse.parse"></a>[function <span class="apidocSignatureSpan">papaparse.</span>parse (_input, _config)](#apidoc.element.papaparse.parse)
- description and source-code
```javascript
function CsvToJson(_input, _config)
	{
		_config = _config || {};
		_config.dynamicTyping = _config.dynamicTyping || false;

		if (_config.worker && Papa.WORKERS_SUPPORTED)
		{
			var w = newWorker();

			w.userStep = _config.step;
			w.userChunk = _config.chunk;
			w.userComplete = _config.complete;
			w.userError = _config.error;

			_config.step = isFunction(_config.step);
			_config.chunk = isFunction(_config.chunk);
			_config.complete = isFunction(_config.complete);
			_config.error = isFunction(_config.error);
			delete _config.worker;	// prevent infinite loop

			w.postMessage({
				input: _input,
				config: _config,
				workerId: w.id
			});

			return;
		}

		var streamer = null;
		if (typeof _input === 'string')
		{
			if (_config.download)
				streamer = new NetworkStreamer(_config);
			else
				streamer = new StringStreamer(_config);
		}
		else if (_input.readable === true && typeof _input.read === 'function' && typeof _input.on === 'function')
		{
			streamer = new ReadableStreamStreamer(_config);
		}
		else if ((global.File && _input instanceof File) || _input instanceof Object)	// ...Safari. (see issue #106)
			streamer = new FileStreamer(_config);

		return streamer.stream(_input);
	}
```
- example usage
```shell
...
				f.instanceConfig.complete = function(results)
				{
					if (isFunction(userCompleteFunc))
						userCompleteFunc(results, f.file, f.inputElem);
					fileComplete();
				};

				Papa.parse(f.file, f.instanceConfig);
			}

			function error(name, file, elem, reason)
			{
				if (isFunction(options.error))
					options.error({name: name}, file, elem, reason);
			}
...
```

#### <a name="apidoc.element.papaparse.unparse"></a>[function <span class="apidocSignatureSpan">papaparse.</span>unparse (_input, _config)](#apidoc.element.papaparse.unparse)
- description and source-code
```javascript
function JsonToCsv(_input, _config)
	{
		var _output = '';
		var _fields = [];

		// Default configuration

		<span class="apidocCodeCommentSpan">/** whether to surround every datum with quotes */
</span>		var _quotes = false;

		/** whether to write headers */
		var _writeHeader = true;

		/** delimiting character */
		var _delimiter = ',';

		/** newline character(s) */
		var _newline = '\r\n';

		/** quote character */
		var _quoteChar = '"';

		unpackConfig();

		var quoteCharRegex = new RegExp(_quoteChar, 'g');

		if (typeof _input === 'string')
			_input = JSON.parse(_input);

		if (_input instanceof Array)
		{
			if (!_input.length || _input[0] instanceof Array)
				return serialize(null, _input);
			else if (typeof _input[0] === 'object')
				return serialize(objectKeys(_input[0]), _input);
		}
		else if (typeof _input === 'object')
		{
			if (typeof _input.data === 'string')
				_input.data = JSON.parse(_input.data);

			if (_input.data instanceof Array)
			{
				if (!_input.fields)
					_input.fields =  _input.meta && _input.meta.fields;

				if (!_input.fields)
					_input.fields =  _input.data[0] instanceof Array
									? _input.fields
									: objectKeys(_input.data[0]);

				if (!(_input.data[0] instanceof Array) && typeof _input.data[0] !== 'object')
					_input.data = [_input.data];	// handles input like [1,2,3] or ['asdf']
			}

			return serialize(_input.fields || [], _input.data || []);
		}

		// Default (any valid paths should return before this)
		throw 'exception: Unable to serialize unrecognized input';


		function unpackConfig()
		{
			if (typeof _config !== 'object')
				return;

			if (typeof _config.delimiter === 'string'
				&& _config.delimiter.length === 1
				&& Papa.BAD_DELIMITERS.indexOf(_config.delimiter) === -1)
			{
				_delimiter = _config.delimiter;
			}

			if (typeof _config.quotes === 'boolean'
				|| _config.quotes instanceof Array)
				_quotes = _config.quotes;

			if (typeof _config.newline === 'string')
				_newline = _config.newline;

			if (typeof _config.quoteChar === 'string')
				_quoteChar = _config.quoteChar;

			if (typeof _config.header === 'boolean')
				_writeHeader = _config.header;
		}


		/** Turns an object's keys into an array */
		function objectKeys(obj)
		{
			if (typeof obj !== 'object')
				return [];
			var keys = [];
			for (var key in obj)
				keys.push(key);
			return keys;
		}

		/** The double for loop that iterates the data and writes out a CSV string including header row */
		function serialize(fields, data)
		{
			var csv = '';

			if (typeof fields === 'string')
				fields = JSON.parse(fields);
			if (typeof data === 'string')
				data = JSON.parse(data);

			var hasHeader = fields instanceof Array && fields.length > 0;
			var dataKeyedByField = !(data[0] instanceof Array);

			// If there a header row, write it first
			if (hasHeader && _writeHeader)
			{
				for (var i = 0; i < fields.length; i++)
				{
					if (i > 0)
						csv += _delimiter;
					csv += safe(fields[i], i);
				}
				if (data.length > 0)
					csv += _newline;
			}

			// Then write out the data
			for (var row = 0; row < data.length; row++)
			{
				var maxCol = hasHeader ? fields.length : data[row].length;

				for (var col = 0; col < maxCol; col++)
				{
					if (col > 0)
						csv += _delimiter;
					var colIdx = hasHeader && dataKeyedByField ? fields[col] : col;
					csv += safe(data[row][colIdx], col);
				}

				if (row < data.length - 1)
					csv += _newline;
			}

			return csv;
		}

		/** Encloses a value around quotes if needed (makes a value safe for CSV insertion) */
		function safe(str, col)
		{
			if (typeof str === 'undefined' || str === null)
				return '';

			str = str.toString().replace(quoteCharRegex, _quoteChar+_quoteChar);

			var needsQuotes = (typeof _quotes === 'boolean' && _quotes)
							|| (_quotes instanceof Array && _quotes[col])
							|| hasAny(str, Papa.BAD_DELIMITERS)
							|| str.indexOf(_delimiter) > -1
							|| str.charAt(0) === ' '
							|| str.charAt(str.length - 1) === ' ';

			return needsQuotes ? _quoteChar + str + _quoteChar : str;
		}

		function hasAny(str, substring ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.papaparse.FileStreamer"></a>[module papaparse.FileStreamer](#apidoc.module.papaparse.FileStreamer)

#### <a name="apidoc.element.papaparse.FileStreamer.FileStreamer"></a>[function <span class="apidocSignatureSpan">papaparse.</span>FileStreamer (config)](#apidoc.element.papaparse.FileStreamer.FileStreamer)
- description and source-code
```javascript
function FileStreamer(config)
	{
		config = config || {};
		if (!config.chunkSize)
			config.chunkSize = Papa.LocalChunkSize;
		ChunkStreamer.call(this, config);

		var reader, slice;

		// FileReader is better than FileReaderSync (even in worker) - see http://stackoverflow.com/q/24708649/1048862
		// But Firefox is a pill, too - see issue #76: https://github.com/mholt/PapaParse/issues/76
		var usingAsyncReader = typeof FileReader !== 'undefined';	// Safari doesn't consider it a function - see issue #105

		this.stream = function(file)
		{
			this._input = file;
			slice = file.slice || file.webkitSlice || file.mozSlice;

			if (usingAsyncReader)
			{
				reader = new FileReader();		// Preferred method of reading files, even in workers
				reader.onload = bindFunction(this._chunkLoaded, this);
				reader.onerror = bindFunction(this._chunkError, this);
			}
			else
				reader = new FileReaderSync();	// Hack for running in a web worker in Firefox

			this._nextChunk();	// Starts streaming
		};

		this._nextChunk = function()
		{
			if (!this._finished && (!this._config.preview || this._rowCount < this._config.preview))
				this._readChunk();
		}

		this._readChunk = function()
		{
			var input = this._input;
			if (this._config.chunkSize)
			{
				var end = Math.min(this._start + this._config.chunkSize, this._input.size);
				input = slice.call(input, this._start, end);
			}
			var txt = reader.readAsText(input, this._config.encoding);
			if (!usingAsyncReader)
				this._chunkLoaded({ target: { result: txt } });	// mimic the async signature
		}

		this._chunkLoaded = function(event)
		{
			// Very important to increment start each time before handling results
			this._start += this._config.chunkSize;
			this._finished = !this._config.chunkSize || this._start >= this._input.size;
			this.parseChunk(event.target.result);
		}

		this._chunkError = function()
		{
			this._sendError(reader.error);
		}

	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.papaparse.FileStreamer.prototype"></a>[module papaparse.FileStreamer.prototype](#apidoc.module.papaparse.FileStreamer.prototype)

#### <a name="apidoc.element.papaparse.FileStreamer.prototype.constructor"></a>[function <span class="apidocSignatureSpan">papaparse.FileStreamer.prototype.</span>constructor (config)](#apidoc.element.papaparse.FileStreamer.prototype.constructor)
- description and source-code
```javascript
function FileStreamer(config)
	{
		config = config || {};
		if (!config.chunkSize)
			config.chunkSize = Papa.LocalChunkSize;
		ChunkStreamer.call(this, config);

		var reader, slice;

		// FileReader is better than FileReaderSync (even in worker) - see http://stackoverflow.com/q/24708649/1048862
		// But Firefox is a pill, too - see issue #76: https://github.com/mholt/PapaParse/issues/76
		var usingAsyncReader = typeof FileReader !== 'undefined';	// Safari doesn't consider it a function - see issue #105

		this.stream = function(file)
		{
			this._input = file;
			slice = file.slice || file.webkitSlice || file.mozSlice;

			if (usingAsyncReader)
			{
				reader = new FileReader();		// Preferred method of reading files, even in workers
				reader.onload = bindFunction(this._chunkLoaded, this);
				reader.onerror = bindFunction(this._chunkError, this);
			}
			else
				reader = new FileReaderSync();	// Hack for running in a web worker in Firefox

			this._nextChunk();	// Starts streaming
		};

		this._nextChunk = function()
		{
			if (!this._finished && (!this._config.preview || this._rowCount < this._config.preview))
				this._readChunk();
		}

		this._readChunk = function()
		{
			var input = this._input;
			if (this._config.chunkSize)
			{
				var end = Math.min(this._start + this._config.chunkSize, this._input.size);
				input = slice.call(input, this._start, end);
			}
			var txt = reader.readAsText(input, this._config.encoding);
			if (!usingAsyncReader)
				this._chunkLoaded({ target: { result: txt } });	// mimic the async signature
		}

		this._chunkLoaded = function(event)
		{
			// Very important to increment start each time before handling results
			this._start += this._config.chunkSize;
			this._finished = !this._config.chunkSize || this._start >= this._input.size;
			this.parseChunk(event.target.result);
		}

		this._chunkError = function()
		{
			this._sendError(reader.error);
		}

	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.papaparse.NetworkStreamer"></a>[module papaparse.NetworkStreamer](#apidoc.module.papaparse.NetworkStreamer)

#### <a name="apidoc.element.papaparse.NetworkStreamer.NetworkStreamer"></a>[function <span class="apidocSignatureSpan">papaparse.</span>NetworkStreamer (config)](#apidoc.element.papaparse.NetworkStreamer.NetworkStreamer)
- description and source-code
```javascript
function NetworkStreamer(config)
	{
		config = config || {};
		if (!config.chunkSize)
			config.chunkSize = Papa.RemoteChunkSize;
		ChunkStreamer.call(this, config);

		var xhr;

		if (IS_WORKER)
		{
			this._nextChunk = function()
			{
				this._readChunk();
				this._chunkLoaded();
			};
		}
		else
		{
			this._nextChunk = function()
			{
				this._readChunk();
			};
		}

		this.stream = function(url)
		{
			this._input = url;
			this._nextChunk();	// Starts streaming
		};

		this._readChunk = function()
		{
			if (this._finished)
			{
				this._chunkLoaded();
				return;
			}

			xhr = new XMLHttpRequest();

			if (this._config.withCredentials)
			{
				xhr.withCredentials = this._config.withCredentials;
			}

			if (!IS_WORKER)
			{
				xhr.onload = bindFunction(this._chunkLoaded, this);
				xhr.onerror = bindFunction(this._chunkError, this);
			}

			xhr.open('GET', this._input, !IS_WORKER);

			if (this._config.chunkSize)
			{
				var end = this._start + this._config.chunkSize - 1;	// minus one because byte range is inclusive
				xhr.setRequestHeader('Range', 'bytes='+this._start+'-'+end);
				xhr.setRequestHeader('If-None-Match', 'webkit-no-cache'); // https://bugs.webkit.org/show_bug.cgi?id=82672
			}

			try {
				xhr.send();
			}
			catch (err) {
				this._chunkError(err.message);
			}

			if (IS_WORKER && xhr.status === 0)
				this._chunkError();
			else
				this._start += this._config.chunkSize;
		}

		this._chunkLoaded = function()
		{
			if (xhr.readyState != 4)
				return;

			if (xhr.status < 200 || xhr.status >= 400)
			{
				this._chunkError();
				return;
			}

			this._finished = !this._config.chunkSize || this._start > getFileSize(xhr);
			this.parseChunk(xhr.responseText);
		}

		this._chunkError = function(errorMessage)
		{
			var errorText = xhr.statusText || errorMessage;
			this._sendError(errorText);
		}

		function getFileSize(xhr)
		{
			var contentRange = xhr.getResponseHeader('Content-Range');
			if (contentRange === null) { // no content range, then finish!
        			return -1;
            		}
			return parseInt(contentRange.substr(contentRange.lastIndexOf('/') + 1));
		}
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.papaparse.NetworkStreamer.prototype"></a>[module papaparse.NetworkStreamer.prototype](#apidoc.module.papaparse.NetworkStreamer.prototype)

#### <a name="apidoc.element.papaparse.NetworkStreamer.prototype.constructor"></a>[function <span class="apidocSignatureSpan">papaparse.NetworkStreamer.prototype.</span>constructor (config)](#apidoc.element.papaparse.NetworkStreamer.prototype.constructor)
- description and source-code
```javascript
function NetworkStreamer(config)
	{
		config = config || {};
		if (!config.chunkSize)
			config.chunkSize = Papa.RemoteChunkSize;
		ChunkStreamer.call(this, config);

		var xhr;

		if (IS_WORKER)
		{
			this._nextChunk = function()
			{
				this._readChunk();
				this._chunkLoaded();
			};
		}
		else
		{
			this._nextChunk = function()
			{
				this._readChunk();
			};
		}

		this.stream = function(url)
		{
			this._input = url;
			this._nextChunk();	// Starts streaming
		};

		this._readChunk = function()
		{
			if (this._finished)
			{
				this._chunkLoaded();
				return;
			}

			xhr = new XMLHttpRequest();

			if (this._config.withCredentials)
			{
				xhr.withCredentials = this._config.withCredentials;
			}

			if (!IS_WORKER)
			{
				xhr.onload = bindFunction(this._chunkLoaded, this);
				xhr.onerror = bindFunction(this._chunkError, this);
			}

			xhr.open('GET', this._input, !IS_WORKER);

			if (this._config.chunkSize)
			{
				var end = this._start + this._config.chunkSize - 1;	// minus one because byte range is inclusive
				xhr.setRequestHeader('Range', 'bytes='+this._start+'-'+end);
				xhr.setRequestHeader('If-None-Match', 'webkit-no-cache'); // https://bugs.webkit.org/show_bug.cgi?id=82672
			}

			try {
				xhr.send();
			}
			catch (err) {
				this._chunkError(err.message);
			}

			if (IS_WORKER && xhr.status === 0)
				this._chunkError();
			else
				this._start += this._config.chunkSize;
		}

		this._chunkLoaded = function()
		{
			if (xhr.readyState != 4)
				return;

			if (xhr.status < 200 || xhr.status >= 400)
			{
				this._chunkError();
				return;
			}

			this._finished = !this._config.chunkSize || this._start > getFileSize(xhr);
			this.parseChunk(xhr.responseText);
		}

		this._chunkError = function(errorMessage)
		{
			var errorText = xhr.statusText || errorMessage;
			this._sendError(errorText);
		}

		function getFileSize(xhr)
		{
			var contentRange = xhr.getResponseHeader('Content-Range');
			if (contentRange === null) { // no content range, then finish!
        			return -1;
            		}
			return parseInt(contentRange.substr(contentRange.lastIndexOf('/') + 1));
		}
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.papaparse.ReadableStreamStreamer"></a>[module papaparse.ReadableStreamStreamer](#apidoc.module.papaparse.ReadableStreamStreamer)

#### <a name="apidoc.element.papaparse.ReadableStreamStreamer.ReadableStreamStreamer"></a>[function <span class="apidocSignatureSpan">papaparse.</span>ReadableStreamStreamer (config)](#apidoc.element.papaparse.ReadableStreamStreamer.ReadableStreamStreamer)
- description and source-code
```javascript
function ReadableStreamStreamer(config)
	{
		config = config || {};

		ChunkStreamer.call(this, config);

		var queue = [];
		var parseOnData = true;

		this.stream = function(stream)
		{
			this._input = stream;

			this._input.on('data', this._streamData);
			this._input.on('end', this._streamEnd);
			this._input.on('error', this._streamError);
		}

		this._nextChunk = function()
		{
			if (queue.length)
			{
				this.parseChunk(queue.shift());
			}
			else
			{
				parseOnData = true;
			}
		}

		this._streamData = bindFunction(function(chunk)
		{
			try
			{
				queue.push(typeof chunk === 'string' ? chunk : chunk.toString(this._config.encoding));

				if (parseOnData)
				{
					parseOnData = false;
					this.parseChunk(queue.shift());
				}
			}
			catch (error)
			{
				this._streamError(error);
			}
		}, this);

		this._streamError = bindFunction(function(error)
		{
			this._streamCleanUp();
			this._sendError(error.message);
		}, this);

		this._streamEnd = bindFunction(function()
		{
			this._streamCleanUp();
			this._finished = true;
			this._streamData('');
		}, this);

		this._streamCleanUp = bindFunction(function()
		{
			this._input.removeListener('data', this._streamData);
			this._input.removeListener('end', this._streamEnd);
			this._input.removeListener('error', this._streamError);
		}, this);
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.papaparse.ReadableStreamStreamer.prototype"></a>[module papaparse.ReadableStreamStreamer.prototype](#apidoc.module.papaparse.ReadableStreamStreamer.prototype)

#### <a name="apidoc.element.papaparse.ReadableStreamStreamer.prototype.constructor"></a>[function <span class="apidocSignatureSpan">papaparse.ReadableStreamStreamer.prototype.</span>constructor (config)](#apidoc.element.papaparse.ReadableStreamStreamer.prototype.constructor)
- description and source-code
```javascript
function ReadableStreamStreamer(config)
	{
		config = config || {};

		ChunkStreamer.call(this, config);

		var queue = [];
		var parseOnData = true;

		this.stream = function(stream)
		{
			this._input = stream;

			this._input.on('data', this._streamData);
			this._input.on('end', this._streamEnd);
			this._input.on('error', this._streamError);
		}

		this._nextChunk = function()
		{
			if (queue.length)
			{
				this.parseChunk(queue.shift());
			}
			else
			{
				parseOnData = true;
			}
		}

		this._streamData = bindFunction(function(chunk)
		{
			try
			{
				queue.push(typeof chunk === 'string' ? chunk : chunk.toString(this._config.encoding));

				if (parseOnData)
				{
					parseOnData = false;
					this.parseChunk(queue.shift());
				}
			}
			catch (error)
			{
				this._streamError(error);
			}
		}, this);

		this._streamError = bindFunction(function(error)
		{
			this._streamCleanUp();
			this._sendError(error.message);
		}, this);

		this._streamEnd = bindFunction(function()
		{
			this._streamCleanUp();
			this._finished = true;
			this._streamData('');
		}, this);

		this._streamCleanUp = bindFunction(function()
		{
			this._input.removeListener('data', this._streamData);
			this._input.removeListener('end', this._streamEnd);
			this._input.removeListener('error', this._streamError);
		}, this);
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.papaparse.StringStreamer"></a>[module papaparse.StringStreamer](#apidoc.module.papaparse.StringStreamer)

#### <a name="apidoc.element.papaparse.StringStreamer.StringStreamer"></a>[function <span class="apidocSignatureSpan">papaparse.</span>StringStreamer (config)](#apidoc.element.papaparse.StringStreamer.StringStreamer)
- description and source-code
```javascript
function StringStreamer(config)
	{
		config = config || {};
		ChunkStreamer.call(this, config);

		var string;
		var remaining;
		this.stream = function(s)
		{
			string = s;
			remaining = s;
			return this._nextChunk();
		}
		this._nextChunk = function()
		{
			if (this._finished) return;
			var size = this._config.chunkSize;
			var chunk = size ? remaining.substr(0, size) : remaining;
			remaining = size ? remaining.substr(size) : '';
			this._finished = !remaining;
			return this.parseChunk(chunk);
		}
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.papaparse.StringStreamer.prototype"></a>[module papaparse.StringStreamer.prototype](#apidoc.module.papaparse.StringStreamer.prototype)

#### <a name="apidoc.element.papaparse.StringStreamer.prototype.constructor"></a>[function <span class="apidocSignatureSpan">papaparse.StringStreamer.prototype.</span>constructor (config)](#apidoc.element.papaparse.StringStreamer.prototype.constructor)
- description and source-code
```javascript
function StringStreamer(config)
	{
		config = config || {};
		ChunkStreamer.call(this, config);

		var string;
		var remaining;
		this.stream = function(s)
		{
			string = s;
			remaining = s;
			return this._nextChunk();
		}
		this._nextChunk = function()
		{
			if (this._finished) return;
			var size = this._config.chunkSize;
			var chunk = size ? remaining.substr(0, size) : remaining;
			remaining = size ? remaining.substr(size) : '';
			this._finished = !remaining;
			return this.parseChunk(chunk);
		}
	}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
