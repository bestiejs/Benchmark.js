# Benchmark.js <sup>v1.0.0</sup>

<!-- div -->


<!-- div -->

## <a id="Benchmark"></a>`Benchmark`
* [`Benchmark`](#benchmarkname-fn--options)
* [`Benchmark.version`](#benchmarkversion)
* [`Benchmark.filter`](#benchmarkfilterarray-callback-thisarg)
* [`Benchmark.formatNumber`](#benchmarkformatnumbernumber)
* [`Benchmark.invoke`](#benchmarkinvokebenches-name--arg)
* [`Benchmark.join`](#benchmarkjoinobject--separator1---separator2:)
* [`Benchmark.runInContext`](#benchmarkrunincontextcontextwindow)

<!-- /div -->


<!-- div -->

## `Benchmark.prototype`
* [`Benchmark.prototype.aborted`](#benchmarkprototypeaborted)
* [`Benchmark.prototype.compiled`](#benchmarkprototypecompiled)
* [`Benchmark.prototype.count`](#benchmarkprototypecount)
* [`Benchmark.prototype.cycles`](#benchmarkprototypecycles)
* [`Benchmark.prototype.error`](#benchmarkprototypeerror)
* [`Benchmark.prototype.fn`](#benchmarkprototypefn)
* [`Benchmark.prototype.hz`](#benchmarkprototypehz)
* [`Benchmark.prototype.running`](#benchmarkprototyperunning)
* [`Benchmark.prototype.setup`](#benchmarkprototypesetup)
* [`Benchmark.prototype.teardown`](#benchmarkprototypeteardown)
* [`Benchmark.prototype.abort`](#benchmarkprototypeabort)
* [`Benchmark.prototype.clone`](#benchmarkprototypecloneoptions)
* [`Benchmark.prototype.compare`](#benchmarkprototypecompareother)
* [`Benchmark.prototype.emit`](#benchmarkprototypeemittype)
* [`Benchmark.prototype.listeners`](#benchmarkprototypelistenerstype)
* [`Benchmark.prototype.off`](#benchmarkprototypeofftype--listener)
* [`Benchmark.prototype.on`](#benchmarkprototypeontype-listener)
* [`Benchmark.prototype.reset`](#benchmarkprototypereset)
* [`Benchmark.prototype.run`](#benchmarkprototyperunoptions)
* [`Benchmark.prototype.toString`](#benchmarkprototypetostring)

<!-- /div -->


<!-- div -->

## `Benchmark.options`
* [`Benchmark.options`](#benchmarkoptions)
* [`Benchmark.options.async`](#benchmarkoptionsasync)
* [`Benchmark.options.defer`](#benchmarkoptionsdefer)
* [`Benchmark.options.delay`](#benchmarkoptionsdelay)
* [`Benchmark.options.id`](#benchmarkoptionsid)
* [`Benchmark.options.initCount`](#benchmarkoptionsinitcount)
* [`Benchmark.options.maxTime`](#benchmarkoptionsmaxtime)
* [`Benchmark.options.minSamples`](#benchmarkoptionsminsamples)
* [`Benchmark.options.minTime`](#benchmarkoptionsmintime)
* [`Benchmark.options.name`](#benchmarkoptionsname)
* [`Benchmark.options.onAbort`](#benchmarkoptionsonabort)
* [`Benchmark.options.onComplete`](#benchmarkoptionsoncomplete)
* [`Benchmark.options.onCycle`](#benchmarkoptionsoncycle)
* [`Benchmark.options.onError`](#benchmarkoptionsonerror)
* [`Benchmark.options.onReset`](#benchmarkoptionsonreset)
* [`Benchmark.options.onStart`](#benchmarkoptionsonstart)

<!-- /div -->


<!-- div -->

## `Benchmark.platform`
* [`Benchmark.platform`](#benchmarkplatform)

<!-- /div -->


<!-- div -->

## `Benchmark.support`
* [`Benchmark.support`](#benchmarksupport)
* [`Benchmark.support.air`](#benchmarksupportair)
* [`Benchmark.support.browser`](#benchmarksupportbrowser)
* [`Benchmark.support.decompilation`](#benchmarksupportdecompilation)
* [`Benchmark.support.java`](#benchmarksupportjava)
* [`Benchmark.support.timeout`](#benchmarksupporttimeout)

<!-- /div -->


<!-- div -->

## `Benchmark.prototype.stats`
* [`Benchmark.prototype.stats`](#benchmarkprototypestats)
* [`Benchmark.prototype.stats.deviation`](#benchmark-statsdeviation)
* [`Benchmark.prototype.stats.mean`](#benchmark-statsmean)
* [`Benchmark.prototype.stats.moe`](#benchmark-statsmoe)
* [`Benchmark.prototype.stats.rme`](#benchmark-statsrme)
* [`Benchmark.prototype.stats.sample`](#benchmark-statssample)
* [`Benchmark.prototype.stats.sem`](#benchmark-statssem)
* [`Benchmark.prototype.stats.variance`](#benchmark-statsvariance)

<!-- /div -->


<!-- div -->

## `Benchmark.prototype.times`
* [`Benchmark.prototype.times`](#benchmarkprototypetimes)
* [`Benchmark.prototype.times.cycle`](#benchmark-timescycle)
* [`Benchmark.prototype.times.elapsed`](#benchmark-timeselapsed)
* [`Benchmark.prototype.times.period`](#benchmark-timesperiod)
* [`Benchmark.prototype.times.timeStamp`](#benchmark-timestimestamp)

<!-- /div -->


<!-- div -->

## `Benchmark.Deferred`
* [`Benchmark.Deferred`](#benchmarkdeferredclone)

<!-- /div -->


<!-- div -->

## `Benchmark.Deferred.prototype`
* [`Benchmark.Deferred.prototype.benchmark`](#benchmarkdeferredprototypebenchmark)
* [`Benchmark.Deferred.prototype.cycles`](#benchmarkdeferredprototypecycles)
* [`Benchmark.Deferred.prototype.elapsed`](#benchmarkdeferredprototypeelapsed)
* [`Benchmark.Deferred.prototype.timeStamp`](#benchmarkdeferredprototypetimestamp)

<!-- /div -->


<!-- div -->

## `Benchmark.Event`
* [`Benchmark.Event`](#benchmarkeventtype)

<!-- /div -->


<!-- div -->

## `Benchmark.Event.prototype`
* [`Benchmark.Event.prototype.aborted`](#benchmarkeventprototypeaborted)
* [`Benchmark.Event.prototype.cancelled`](#benchmarkeventprototypecancelled)
* [`Benchmark.Event.prototype.currentTarget`](#benchmarkeventprototypecurrenttarget)
* [`Benchmark.Event.prototype.result`](#benchmarkeventprototyperesult)
* [`Benchmark.Event.prototype.target`](#benchmarkeventprototypetarget)
* [`Benchmark.Event.prototype.timeStamp`](#benchmarkeventprototypetimestamp)
* [`Benchmark.Event.prototype.type`](#benchmarkeventprototypetype)

<!-- /div -->


<!-- div -->

## `Benchmark.Suite`
* [`Benchmark.Suite`](#benchmarksuitename--options)

<!-- /div -->


<!-- div -->

## `Benchmark.Suite.prototype`
* [`Benchmark.Suite.prototype.aborted`](#benchmarksuiteprototypeaborted)
* [`Benchmark.Suite.prototype.length`](#benchmarksuiteprototypelength)
* [`Benchmark.Suite.prototype.running`](#benchmarksuiteprototyperunning)
* [`Benchmark.Suite.prototype.abort`](#benchmarksuiteprototypeabort)
* [`Benchmark.Suite.prototype.add`](#benchmarksuiteprototypeaddname-fn--options)
* [`Benchmark.Suite.prototype.clone`](#benchmarksuiteprototypecloneoptions)
* [`Benchmark.Suite.prototype.emit`](#benchmarkprototypeemittype)
* [`Benchmark.Suite.prototype.filter`](#benchmarksuiteprototypefiltercallback)
* [`Benchmark.Suite.prototype.listeners`](#benchmarkprototypelistenerstype)
* [`Benchmark.Suite.prototype.off`](#benchmarkprototypeofftype--listener)
* [`Benchmark.Suite.prototype.on`](#benchmarkprototypeontype-listener)
* [`Benchmark.Suite.prototype.reset`](#benchmarksuiteprototypereset)
* [`Benchmark.Suite.prototype.run`](#benchmarksuiteprototyperunoptions)

<!-- /div -->


<!-- div -->

## `Benchmark.Suite.options`
* [`Benchmark.Suite.options`](#benchmarksuiteoptions)
* [`Benchmark.Suite.options.name`](#benchmarksuiteoptionsname)

<!-- /div -->


<!-- /div -->


<!-- div -->


<!-- div -->

## `Benchmark`

<!-- div -->

### <a id="benchmarkname-fn--options"></a>`Benchmark(name, fn, [options={}])`
<a href="#benchmarkname-fn--options">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L356 "View in source") [&#x24C9;][1]

The Benchmark constructor.

#### Arguments
1. `name` *(string)*: A name to identify the benchmark.
2. `fn` *(function|string)*: The test to benchmark.
3. `[options={}]` *(object)*: Options object.

#### Example
```js
// basic usage (the `new` operator is optional)
var bench = new Benchmark(fn);

// or using a name first
var bench = new Benchmark('foo', fn);

// or with options
var bench = new Benchmark('foo', fn, {

  // displayed by Benchmark#toString if `name` is not available
  'id': 'xyz',

  // called when the benchmark starts running
  'onStart': onStart,

  // called after each run cycle
  'onCycle': onCycle,

  // called when aborted
  'onAbort': onAbort,

  // called when a test errors
  'onError': onError,

  // called when reset
  'onReset': onReset,

  // called when the benchmark completes running
  'onComplete': onComplete,

  // compiled/called before the test loop
  'setup': setup,

  // compiled/called after the test loop
  'teardown': teardown
});

// or name and options
var bench = new Benchmark('foo', {

  // a flag to indicate the benchmark is deferred
  'defer': true,

  // benchmark test function
  'fn': function(deferred) {
    // call resolve() when the deferred test is finished
    deferred.resolve();
  }
});

// or options only
var bench = new Benchmark({

  // benchmark name
  'name': 'foo',

  // benchmark test as a string
  'fn': '[1,2,3,4].sort()'
});

// a test's `this` binding is set to the benchmark instance
var bench = new Benchmark('foo', function() {
  'My name is '.concat(this.name); // My name is foo
});
```

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkversion"></a>`Benchmark.version`
<a href="#benchmarkversion">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2347 "View in source") [&#x24C9;][1]

*(string)*: The semantic version number.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkfilterarray-callback-thisarg"></a>`Benchmark.filter(array, callback, thisArg)`
<a href="#benchmarkfilterarray-callback-thisarg">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L781 "View in source") [&#x24C9;][1]

A generic `Array#filter` like method.

#### Arguments
1. `array` *(array)*: The array to iterate over.
2. `callback` *(function|string)*: The function/alias called per iteration.
3. `thisArg` *(\*)*: The `this` binding for the callback.

#### Returns
*(array)*: A new array of values that passed callback filter.

#### Example
```js
// get odd numbers
Benchmark.filter([1, 2, 3, 4, 5], function(n) {
  return n % 2;
}); // -> [1, 3, 5];

// get fastest benchmarks
Benchmark.filter(benches, 'fastest');

// get slowest benchmarks
Benchmark.filter(benches, 'slowest');

// get benchmarks that completed without erroring
Benchmark.filter(benches, 'successful');
```

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkformatnumbernumber"></a>`Benchmark.formatNumber(number)`
<a href="#benchmarkformatnumbernumber">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L810 "View in source") [&#x24C9;][1]

Converts a number to a more readable comma-separated string representation.

#### Arguments
1. `number` *(number)*: The number to convert.

#### Returns
*(string)*: The more readable string representation.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkinvokebenches-name--arg"></a>`Benchmark.invoke(benches, name, [arg])`
<a href="#benchmarkinvokebenches-name--arg">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L855 "View in source") [&#x24C9;][1]

Invokes a method on all items in an array.

#### Arguments
1. `benches` *(array)*: Array of benchmarks to iterate over.
2. `name` *(object|string)*: The name of the method to invoke OR options object.
3. `[arg]` *(...\*)*: Arguments to invoke the method with.

#### Returns
*(array)*: A new array of values returned from each method invoked.

#### Example
```js
// invoke `reset` on all benchmarks
Benchmark.invoke(benches, 'reset');

// invoke `emit` with arguments
Benchmark.invoke(benches, 'emit', 'complete', listener);

// invoke `run(true)`, treat benchmarks as a queue, and register invoke callbacks
Benchmark.invoke(benches, {

  // invoke the `run` method
  'name': 'run',

  // pass a single argument
  'args': true,

  // treat as queue, removing benchmarks from front of `benches` until empty
  'queued': true,

  // called before any benchmarks have been invoked.
  'onStart': onStart,

  // called between invoking benchmarks
  'onCycle': onCycle,

  // called after all benchmarks have been invoked.
  'onComplete': onComplete
});
```

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkjoinobject--separator1---separator2:"></a>`Benchmark.join(object, [separator1=','], [separator2=': '])`
<a href="#benchmarkjoinobject--separator1---separator2:">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1007 "View in source") [&#x24C9;][1]

Creates a string of joined array values or object key-value pairs.

#### Arguments
1. `object` *(array|object)*: The object to operate on.
2. `[separator1=',']` *(string)*: The separator used between key-value pairs.
3. `[separator2=': ']` *(string)*: The separator used between keys and values.

#### Returns
*(string)*: The joined result.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkrunincontextcontextwindow"></a>`Benchmark.runInContext([context=window])`
<a href="#benchmarkrunincontextcontextwindow">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L111 "View in source") [&#x24C9;][1]

Create a new `Benchmark` function using the given `context` object.

#### Arguments
1. `[context=window]` *(object)*: The context object.

#### Returns
*(function)*: Returns the `Benchmark` function.

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.prototype`

<!-- div -->

### <a id="benchmarkprototypeaborted"></a>`Benchmark.prototype.aborted`
<a href="#benchmarkprototypeaborted">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2422 "View in source") [&#x24C9;][1]

*(boolean)*: A flag to indicate if the benchmark is aborted.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypecompiled"></a>`Benchmark.prototype.compiled`
<a href="#benchmarkprototypecompiled">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2398 "View in source") [&#x24C9;][1]

*(function, ...string)*: The compiled test function.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypecount"></a>`Benchmark.prototype.count`
<a href="#benchmarkprototypecount">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2374 "View in source") [&#x24C9;][1]

*(number)*: The number of times a test was executed.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypecycles"></a>`Benchmark.prototype.cycles`
<a href="#benchmarkprototypecycles">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2382 "View in source") [&#x24C9;][1]

*(number)*: The number of cycles performed while benchmarking.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypeerror"></a>`Benchmark.prototype.error`
<a href="#benchmarkprototypeerror">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2406 "View in source") [&#x24C9;][1]

*(object)*: The error object if the test failed.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypefn"></a>`Benchmark.prototype.fn`
<a href="#benchmarkprototypefn">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2414 "View in source") [&#x24C9;][1]

*(function, ...string)*: The test to benchmark.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypehz"></a>`Benchmark.prototype.hz`
<a href="#benchmarkprototypehz">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2390 "View in source") [&#x24C9;][1]

*(number)*: The number of executions per second.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototyperunning"></a>`Benchmark.prototype.running`
<a href="#benchmarkprototyperunning">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2430 "View in source") [&#x24C9;][1]

*(boolean)*: A flag to indicate if the benchmark is running.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypesetup"></a>`Benchmark.prototype.setup`
<a href="#benchmarkprototypesetup">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2493 "View in source") [&#x24C9;][1]

*(function, ...string)*: Compiled into the test and executed immediately **before** the test loop.

#### Example
```js
// basic usage
var bench = Benchmark({
  'setup': function() {
    var c = this.count,
        element = document.getElementById('container');
    while (c--) {
      element.appendChild(document.createElement('div'));
    }
  },
  'fn': function() {
    element.removeChild(element.lastChild);
  }
});

// compiles to something like:
var c = this.count,
    element = document.getElementById('container');
while (c--) {
  element.appendChild(document.createElement('div'));
}
var start = new Date;
while (count--) {
  element.removeChild(element.lastChild);
}
var end = new Date - start;

// or using strings
var bench = Benchmark({
  'setup': '\
    var a = 0;\n\
    (function() {\n\
      (function() {\n\
        (function() {',
  'fn': 'a += 1;',
  'teardown': '\
         }())\n\
       }())\n\
     }())'
});

// compiles to something like:
var a = 0;
(function() {
  (function() {
    (function() {
      var start = new Date;
      while (count--) {
        a += 1;
      }
      var end = new Date - start;
    }())
  }())
}())
```

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypeteardown"></a>`Benchmark.prototype.teardown`
<a href="#benchmarkprototypeteardown">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2501 "View in source") [&#x24C9;][1]

*(function, ...string)*: Compiled into the test and executed immediately **after** the test loop.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypeabort"></a>`Benchmark.prototype.abort()`
<a href="#benchmarkprototypeabort">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1347 "View in source") [&#x24C9;][1]

Aborts the benchmark without recording times.

#### Returns
*(object)*: The benchmark instance.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypecloneoptions"></a>`Benchmark.prototype.clone(options)`
<a href="#benchmarkprototypecloneoptions">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1386 "View in source") [&#x24C9;][1]

Creates a new benchmark using the same test and options.

#### Arguments
1. `options` *(object)*: Options object to overwrite cloned options.

#### Returns
*(object)*: The new benchmark instance.

#### Example
```js
var bizarro = bench.clone({
  'name': 'doppelganger'
});
```

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypecompareother"></a>`Benchmark.prototype.compare(other)`
<a href="#benchmarkprototypecompareother">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1411 "View in source") [&#x24C9;][1]

Determines if a benchmark is faster than another.

#### Arguments
1. `other` *(object)*: The benchmark to compare.

#### Returns
*(number)*: Returns `-1` if slower, `1` if faster, and `0` if indeterminate.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypeemittype"></a>`Benchmark.Suite.prototype.emit(type)`
<a href="#benchmarkprototypeemittype">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1221 "View in source") [&#x24C9;][1]

Executes all registered listeners of the specified event type.

#### Arguments
1. `type` *(object|string)*: The event type or object.

#### Returns
*(\*)*: Returns the return value of the last listener executed.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypelistenerstype"></a>`Benchmark.Suite.prototype.listeners(type)`
<a href="#benchmarkprototypelistenerstype">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1251 "View in source") [&#x24C9;][1]

Returns an array of event listeners for a given type that can be manipulated to add or remove listeners.

#### Arguments
1. `type` *(string)*: The event type.

#### Returns
*(array)*: The listeners array.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypeofftype--listener"></a>`Benchmark.Suite.prototype.off([type], [listener])`
<a href="#benchmarkprototypeofftype--listener">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1284 "View in source") [&#x24C9;][1]

Unregisters a listener for the specified event type(s), or unregisters all listeners for the specified event type(s), or unregisters all listeners for all event types.

#### Arguments
1. `[type]` *(string)*: The event type.
2. `[listener]` *(function)*: The function to unregister.

#### Returns
*(object)*: The benchmark instance.

#### Example
```js
// unregister a listener for an event type
bench.off('cycle', listener);

// unregister a listener for multiple event types
bench.off('start cycle', listener);

// unregister all listeners for an event type
bench.off('cycle');

// unregister all listeners for multiple event types
bench.off('start cycle complete');

// unregister all listeners for all event types
bench.off();
```

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypeontype-listener"></a>`Benchmark.Suite.prototype.on(type, listener)`
<a href="#benchmarkprototypeontype-listener">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1326 "View in source") [&#x24C9;][1]

Registers a listener for the specified event type(s).

#### Arguments
1. `type` *(string)*: The event type.
2. `listener` *(function)*: The function to register.

#### Returns
*(object)*: The benchmark instance.

#### Example
```js
// register a listener for an event type
bench.on('cycle', listener);

// register a listener for multiple event types
bench.on('start cycle', listener);
```

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypereset"></a>`Benchmark.prototype.reset()`
<a href="#benchmarkprototypereset">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1464 "View in source") [&#x24C9;][1]

Reset properties and abort if running.

#### Returns
*(object)*: The benchmark instance.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototyperunoptions"></a>`Benchmark.prototype.run([options={}])`
<a href="#benchmarkprototyperunoptions">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2143 "View in source") [&#x24C9;][1]

Runs the benchmark.

#### Arguments
1. `[options={}]` *(object)*: Options object.

#### Returns
*(object)*: The benchmark instance.

#### Example
```js
// basic usage
bench.run();

// or with options
bench.run({ 'async': true });
```

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypetostring"></a>`Benchmark.prototype.toString()`
<a href="#benchmarkprototypetostring">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1535 "View in source") [&#x24C9;][1]

Displays relevant benchmark information when coerced to a string.

#### Returns
*(string)*: A string representation of the benchmark instance.

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.options`

<!-- div -->

### <a id="benchmarkoptions"></a>`Benchmark.options`
<a href="#benchmarkoptions">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2192 "View in source") [&#x24C9;][1]

*(object)*: The default options copied by benchmark instances.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsasync"></a>`Benchmark.options.async`
<a href="#benchmarkoptionsasync">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2201 "View in source") [&#x24C9;][1]

*(boolean)*: A flag to indicate that benchmark cycles will execute asynchronously by default.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsdefer"></a>`Benchmark.options.defer`
<a href="#benchmarkoptionsdefer">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2209 "View in source") [&#x24C9;][1]

*(boolean)*: A flag to indicate that the benchmark clock is deferred.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsdelay"></a>`Benchmark.options.delay`
<a href="#benchmarkoptionsdelay">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2216 "View in source") [&#x24C9;][1]

*(number)*: The delay between test cycles *(secs)*.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsid"></a>`Benchmark.options.id`
<a href="#benchmarkoptionsid">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2225 "View in source") [&#x24C9;][1]

*(string)*: Displayed by Benchmark#toString when a `name` is not available *(auto-generated if absent)*.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsinitcount"></a>`Benchmark.options.initCount`
<a href="#benchmarkoptionsinitcount">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2233 "View in source") [&#x24C9;][1]

*(number)*: The default number of times to execute a test on a benchmark's first cycle.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsmaxtime"></a>`Benchmark.options.maxTime`
<a href="#benchmarkoptionsmaxtime">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2243 "View in source") [&#x24C9;][1]

*(number)*: The maximum time a benchmark is allowed to run before finishing *(secs)*.

Note: Cycle delays aren't counted toward the maximum time.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsminsamples"></a>`Benchmark.options.minSamples`
<a href="#benchmarkoptionsminsamples">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2251 "View in source") [&#x24C9;][1]

*(number)*: The minimum sample size required to perform statistical analysis.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsmintime"></a>`Benchmark.options.minTime`
<a href="#benchmarkoptionsmintime">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2259 "View in source") [&#x24C9;][1]

*(number)*: The time needed to reduce the percent uncertainty of measurement to `1`% *(secs)*.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsname"></a>`Benchmark.options.name`
<a href="#benchmarkoptionsname">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2267 "View in source") [&#x24C9;][1]

*(string)*: The name of the benchmark.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsonabort"></a>`Benchmark.options.onAbort`
<a href="#benchmarkoptionsonabort">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2275 "View in source") [&#x24C9;][1]

An event listener called when the benchmark is aborted.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsoncomplete"></a>`Benchmark.options.onComplete`
<a href="#benchmarkoptionsoncomplete">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2283 "View in source") [&#x24C9;][1]

An event listener called when the benchmark completes running.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsoncycle"></a>`Benchmark.options.onCycle`
<a href="#benchmarkoptionsoncycle">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2291 "View in source") [&#x24C9;][1]

An event listener called after each run cycle.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsonerror"></a>`Benchmark.options.onError`
<a href="#benchmarkoptionsonerror">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2299 "View in source") [&#x24C9;][1]

An event listener called when a test errors.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsonreset"></a>`Benchmark.options.onReset`
<a href="#benchmarkoptionsonreset">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2307 "View in source") [&#x24C9;][1]

An event listener called when the benchmark is reset.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkoptionsonstart"></a>`Benchmark.options.onStart`
<a href="#benchmarkoptionsonstart">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2315 "View in source") [&#x24C9;][1]

An event listener called when the benchmark starts running.

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.platform`

<!-- div -->

### <a id="benchmarkplatform"></a>`Benchmark.platform`
<a href="#benchmarkplatform">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2326 "View in source") [&#x24C9;][1]

*(object)*: Platform object with properties describing things like browser name, version, and operating system.

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.support`

<!-- div -->

### <a id="benchmarksupport"></a>`Benchmark.support`
<a href="#benchmarksupport">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L186 "View in source") [&#x24C9;][1]

*(object)*: An object used to flag environments/features.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksupportair"></a>`Benchmark.support.air`
<a href="#benchmarksupportair">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L196 "View in source") [&#x24C9;][1]

*(boolean)*: Detect Adobe AIR.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksupportbrowser"></a>`Benchmark.support.browser`
<a href="#benchmarksupportbrowser">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L204 "View in source") [&#x24C9;][1]

*(boolean)*: Detect if in a browser environment.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksupportdecompilation"></a>`Benchmark.support.decompilation`
<a href="#benchmarksupportdecompilation">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L229 "View in source") [&#x24C9;][1]

*(boolean)*: Detect if functions support decompilation.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksupportjava"></a>`Benchmark.support.java`
<a href="#benchmarksupportjava">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L212 "View in source") [&#x24C9;][1]

*(boolean)*: Detect if Java is enabled/exposed.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksupporttimeout"></a>`Benchmark.support.timeout`
<a href="#benchmarksupporttimeout">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L220 "View in source") [&#x24C9;][1]

*(boolean)*: Detect if the Timers API exists.

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.prototype.stats`

<!-- div -->

### <a id="benchmarkprototypestats"></a>`Benchmark.prototype.stats`
<a href="#benchmarkprototypestats">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2509 "View in source") [&#x24C9;][1]

*(object)*: An object of stats including mean, margin or error, and standard deviation.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmark-statsdeviation"></a>`Benchmark.prototype.stats.deviation`
<a href="#benchmark-statsdeviation">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2541 "View in source") [&#x24C9;][1]

*(number)*: The sample standard deviation.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmark-statsmean"></a>`Benchmark.prototype.stats.mean`
<a href="#benchmark-statsmean">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2549 "View in source") [&#x24C9;][1]

*(number)*: The sample arithmetic mean *(secs)*.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmark-statsmoe"></a>`Benchmark.prototype.stats.moe`
<a href="#benchmark-statsmoe">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2517 "View in source") [&#x24C9;][1]

*(number)*: The margin of error.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmark-statsrme"></a>`Benchmark.prototype.stats.rme`
<a href="#benchmark-statsrme">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2525 "View in source") [&#x24C9;][1]

*(number)*: The relative margin of error *(expressed as a percentage of the mean)*.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmark-statssample"></a>`Benchmark.prototype.stats.sample`
<a href="#benchmark-statssample">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2557 "View in source") [&#x24C9;][1]

*(array)*: The array of sampled periods.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmark-statssem"></a>`Benchmark.prototype.stats.sem`
<a href="#benchmark-statssem">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2533 "View in source") [&#x24C9;][1]

*(number)*: The standard error of the mean.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmark-statsvariance"></a>`Benchmark.prototype.stats.variance`
<a href="#benchmark-statsvariance">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2565 "View in source") [&#x24C9;][1]

*(number)*: The sample variance.

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.prototype.times`

<!-- div -->

### <a id="benchmarkprototypetimes"></a>`Benchmark.prototype.times`
<a href="#benchmarkprototypetimes">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2574 "View in source") [&#x24C9;][1]

*(object)*: An object of timing data including cycle, elapsed, period, start, and stop.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmark-timescycle"></a>`Benchmark.prototype.times.cycle`
<a href="#benchmark-timescycle">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2582 "View in source") [&#x24C9;][1]

*(number)*: The time taken to complete the last cycle *(secs)*.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmark-timeselapsed"></a>`Benchmark.prototype.times.elapsed`
<a href="#benchmark-timeselapsed">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2590 "View in source") [&#x24C9;][1]

*(number)*: The time taken to complete the benchmark *(secs)*.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmark-timesperiod"></a>`Benchmark.prototype.times.period`
<a href="#benchmark-timesperiod">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2598 "View in source") [&#x24C9;][1]

*(number)*: The time taken to execute the test once *(secs)*.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmark-timestimestamp"></a>`Benchmark.prototype.times.timeStamp`
<a href="#benchmark-timestimestamp">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2606 "View in source") [&#x24C9;][1]

*(number)*: A timestamp of when the benchmark started *(ms)*.

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.Deferred`

<!-- div -->

### <a id="benchmarkdeferredclone"></a>`Benchmark.Deferred(clone)`
<a href="#benchmarkdeferredclone">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L399 "View in source") [&#x24C9;][1]

The Deferred constructor.

#### Arguments
1. `clone` *(object)*: The cloned benchmark instance.

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.Deferred.prototype`

<!-- div -->

### <a id="benchmarkdeferredprototypebenchmark"></a>`Benchmark.Deferred.prototype.benchmark`
<a href="#benchmarkdeferredprototypebenchmark">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2633 "View in source") [&#x24C9;][1]

*(object)*: The deferred benchmark instance.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkdeferredprototypecycles"></a>`Benchmark.Deferred.prototype.cycles`
<a href="#benchmarkdeferredprototypecycles">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2641 "View in source") [&#x24C9;][1]

*(number)*: The number of deferred cycles performed while benchmarking.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkdeferredprototypeelapsed"></a>`Benchmark.Deferred.prototype.elapsed`
<a href="#benchmarkdeferredprototypeelapsed">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2649 "View in source") [&#x24C9;][1]

*(number)*: The time taken to complete the deferred benchmark *(secs)*.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkdeferredprototypetimestamp"></a>`Benchmark.Deferred.prototype.timeStamp`
<a href="#benchmarkdeferredprototypetimestamp">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2657 "View in source") [&#x24C9;][1]

*(number)*: A timestamp of when the deferred benchmark started *(ms)*.

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.Event`

<!-- div -->

### <a id="benchmarkeventtype"></a>`Benchmark.Event(type)`
<a href="#benchmarkeventtype">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L415 "View in source") [&#x24C9;][1]

The Event constructor.

#### Arguments
1. `type` *(object|string)*: The event type.

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.Event.prototype`

<!-- div -->

### <a id="benchmarkeventprototypeaborted"></a>`Benchmark.Event.prototype.aborted`
<a href="#benchmarkeventprototypeaborted">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2674 "View in source") [&#x24C9;][1]

*(boolean)*: A flag to indicate if the emitters listener iteration is aborted.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkeventprototypecancelled"></a>`Benchmark.Event.prototype.cancelled`
<a href="#benchmarkeventprototypecancelled">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2682 "View in source") [&#x24C9;][1]

*(boolean)*: A flag to indicate if the default action is cancelled.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkeventprototypecurrenttarget"></a>`Benchmark.Event.prototype.currentTarget`
<a href="#benchmarkeventprototypecurrenttarget">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2690 "View in source") [&#x24C9;][1]

*(object)*: The object whose listeners are currently being processed.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkeventprototyperesult"></a>`Benchmark.Event.prototype.result`
<a href="#benchmarkeventprototyperesult">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2698 "View in source") [&#x24C9;][1]

*(mixed)*: The return value of the last executed listener.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkeventprototypetarget"></a>`Benchmark.Event.prototype.target`
<a href="#benchmarkeventprototypetarget">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2706 "View in source") [&#x24C9;][1]

*(object)*: The object to which the event was originally emitted.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkeventprototypetimestamp"></a>`Benchmark.Event.prototype.timeStamp`
<a href="#benchmarkeventprototypetimestamp">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2714 "View in source") [&#x24C9;][1]

*(number)*: A timestamp of when the event was created *(ms)*.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkeventprototypetype"></a>`Benchmark.Event.prototype.type`
<a href="#benchmarkeventprototypetype">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2722 "View in source") [&#x24C9;][1]

*(string)*: The event type.

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.Suite`

<!-- div -->

### <a id="benchmarksuitename--options"></a>`Benchmark.Suite(name, [options={}])`
<a href="#benchmarksuitename--options">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L462 "View in source") [&#x24C9;][1]

The Suite constructor.

#### Arguments
1. `name` *(string)*: A name to identify the suite.
2. `[options={}]` *(object)*: Options object.

#### Example
```js
// basic usage (the `new` operator is optional)
var suite = new Benchmark.Suite;

// or using a name first
var suite = new Benchmark.Suite('foo');

// or with options
var suite = new Benchmark.Suite('foo', {

  // called when the suite starts running
  'onStart': onStart,

  // called between running benchmarks
  'onCycle': onCycle,

  // called when aborted
  'onAbort': onAbort,

  // called when a test errors
  'onError': onError,

  // called when reset
  'onReset': onReset,

  // called when the suite completes running
  'onComplete': onComplete
});
```

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.Suite.prototype`

<!-- div -->

### <a id="benchmarksuiteprototypeaborted"></a>`Benchmark.Suite.prototype.aborted`
<a href="#benchmarksuiteprototypeaborted">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2763 "View in source") [&#x24C9;][1]

*(boolean)*: A flag to indicate if the suite is aborted.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksuiteprototypelength"></a>`Benchmark.Suite.prototype.length`
<a href="#benchmarksuiteprototypelength">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2755 "View in source") [&#x24C9;][1]

*(number)*: The number of benchmarks in the suite.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksuiteprototyperunning"></a>`Benchmark.Suite.prototype.running`
<a href="#benchmarksuiteprototyperunning">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2771 "View in source") [&#x24C9;][1]

*(boolean)*: A flag to indicate if the suite is running.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksuiteprototypeabort"></a>`Benchmark.Suite.prototype.abort()`
<a href="#benchmarksuiteprototypeabort">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1028 "View in source") [&#x24C9;][1]

Aborts all benchmarks in the suite.

#### Returns
*(object)*: The suite instance.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksuiteprototypeaddname-fn--options"></a>`Benchmark.Suite.prototype.add(name, fn, [options={}])`
<a href="#benchmarksuiteprototypeaddname-fn--options">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1088 "View in source") [&#x24C9;][1]

Adds a test to the benchmark suite.

#### Arguments
1. `name` *(string)*: A name to identify the benchmark.
2. `fn` *(function|string)*: The test to benchmark.
3. `[options={}]` *(object)*: Options object.

#### Returns
*(object)*: The benchmark instance.

#### Example
```js
// basic usage
suite.add(fn);

// or using a name first
suite.add('foo', fn);

// or with options
suite.add('foo', fn, {
  'onCycle': onCycle,
  'onComplete': onComplete
});

// or name and options
suite.add('foo', {
  'fn': fn,
  'onCycle': onCycle,
  'onComplete': onComplete
});

// or options only
suite.add({
  'name': 'foo',
  'fn': fn,
  'onCycle': onCycle,
  'onComplete': onComplete
});
```

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksuiteprototypecloneoptions"></a>`Benchmark.Suite.prototype.clone(options)`
<a href="#benchmarksuiteprototypecloneoptions">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1107 "View in source") [&#x24C9;][1]

Creates a new suite with cloned benchmarks.

#### Arguments
1. `options` *(object)*: Options object to overwrite cloned options.

#### Returns
*(object)*: The new suite instance.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypeemittype"></a>`Benchmark.Suite.prototype.emit(type)`
<a href="#benchmarkprototypeemittype">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1221 "View in source") [&#x24C9;][1]

Executes all registered listeners of the specified event type.

#### Arguments
1. `type` *(object|string)*: The event type or object.

#### Returns
*(\*)*: Returns the return value of the last listener executed.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksuiteprototypefiltercallback"></a>`Benchmark.Suite.prototype.filter(callback)`
<a href="#benchmarksuiteprototypefiltercallback">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1130 "View in source") [&#x24C9;][1]

An `Array#filter` like method.

#### Arguments
1. `callback` *(function|string)*: The function/alias called per iteration.

#### Returns
*(object)*: A new suite of benchmarks that passed callback filter.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypelistenerstype"></a>`Benchmark.Suite.prototype.listeners(type)`
<a href="#benchmarkprototypelistenerstype">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1251 "View in source") [&#x24C9;][1]

Returns an array of event listeners for a given type that can be manipulated to add or remove listeners.

#### Arguments
1. `type` *(string)*: The event type.

#### Returns
*(array)*: The listeners array.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypeofftype--listener"></a>`Benchmark.Suite.prototype.off([type], [listener])`
<a href="#benchmarkprototypeofftype--listener">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1284 "View in source") [&#x24C9;][1]

Unregisters a listener for the specified event type(s), or unregisters all listeners for the specified event type(s), or unregisters all listeners for all event types.

#### Arguments
1. `[type]` *(string)*: The event type.
2. `[listener]` *(function)*: The function to unregister.

#### Returns
*(object)*: The benchmark instance.

#### Example
```js
// unregister a listener for an event type
bench.off('cycle', listener);

// unregister a listener for multiple event types
bench.off('start cycle', listener);

// unregister all listeners for an event type
bench.off('cycle');

// unregister all listeners for multiple event types
bench.off('start cycle complete');

// unregister all listeners for all event types
bench.off();
```

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarkprototypeontype-listener"></a>`Benchmark.Suite.prototype.on(type, listener)`
<a href="#benchmarkprototypeontype-listener">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1326 "View in source") [&#x24C9;][1]

Registers a listener for the specified event type(s).

#### Arguments
1. `type` *(string)*: The event type.
2. `listener` *(function)*: The function to register.

#### Returns
*(object)*: The benchmark instance.

#### Example
```js
// register a listener for an event type
bench.on('cycle', listener);

// register a listener for multiple event types
bench.on('start cycle', listener);
```

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksuiteprototypereset"></a>`Benchmark.Suite.prototype.reset()`
<a href="#benchmarksuiteprototypereset">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1145 "View in source") [&#x24C9;][1]

Resets all benchmarks in the suite.

#### Returns
*(object)*: The suite instance.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksuiteprototyperunoptions"></a>`Benchmark.Suite.prototype.run([options={}])`
<a href="#benchmarksuiteprototyperunoptions">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L1182 "View in source") [&#x24C9;][1]

Runs the suite.

#### Arguments
1. `[options={}]` *(object)*: Options object.

#### Returns
*(object)*: The suite instance.

#### Example
```js
// basic usage
suite.run();

// or with options
suite.run({ 'async': true, 'queued': true });
```

* * *

<!-- /div -->


<!-- /div -->


<!-- div -->

## `Benchmark.Suite.options`

<!-- div -->

### <a id="benchmarksuiteoptions"></a>`Benchmark.Suite.options`
<a href="#benchmarksuiteoptions">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2734 "View in source") [&#x24C9;][1]

*(object)*: The default options copied by suite instances.

* * *

<!-- /div -->


<!-- div -->

### <a id="benchmarksuiteoptionsname"></a>`Benchmark.Suite.options.name`
<a href="#benchmarksuiteoptionsname">#</a> [&#x24C8;](https://github.com/bestiejs/benchmark.js/blob/master/benchmark.js#L2742 "View in source") [&#x24C9;][1]

*(string)*: The name of the suite.

* * *

<!-- /div -->


<!-- /div -->


<!-- /div -->


  [1]: #Benchmark "Jump back to the TOC."