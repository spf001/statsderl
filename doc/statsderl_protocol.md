

# Module statsderl_protocol #
* [Data Types](#types)
* [Function Index](#index)
* [Function Details](#functions)

<a name="types"></a>

## Data Types ##




### <a name="type-key">key()</a> ###


<pre><code>
key() = iodata()
</code></pre>




### <a name="type-operation">operation()</a> ###


<pre><code>
operation() = {cast, iodata()} | {counter, <a href="#type-key">key()</a>, <a href="#type-value">value()</a>, <a href="#type-sample_rate">sample_rate()</a>} | {gauge, <a href="#type-key">key()</a>, <a href="#type-value">value()</a>} | {gauge_decrement, <a href="#type-key">key()</a>, <a href="#type-value">value()</a>} | {gauge_increment, <a href="#type-key">key()</a>, <a href="#type-value">value()</a>} | {timing, <a href="#type-key">key()</a>, <a href="#type-value">value()</a>} | {timing_now, <a href="#type-key">key()</a>, <a href="erlang.md#type-timestamp">erlang:timestamp()</a>} | {timing_now_us, <a href="#type-key">key()</a>, <a href="erlang.md#type-timestamp">erlang:timestamp()</a>}
</code></pre>




### <a name="type-sample_rate">sample_rate()</a> ###


<pre><code>
sample_rate() = number()
</code></pre>




### <a name="type-value">value()</a> ###


<pre><code>
value() = number()
</code></pre>

<a name="index"></a>

## Function Index ##


<table width="100%" border="1" cellspacing="0" cellpadding="2" summary="function index"><tr><td valign="top"><a href="#encode-1">encode/1</a></td><td></td></tr></table>


<a name="functions"></a>

## Function Details ##

<a name="encode-1"></a>

### encode/1 ###

<pre><code>
encode(X1::<a href="#type-operation">operation()</a>) -&gt; iodata()
</code></pre>
<br />

