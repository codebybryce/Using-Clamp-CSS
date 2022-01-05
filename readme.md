# CSS clamp() and min() max()

## Code pen
```
<div class="codepen" data-height="300" data-theme-id="dark" data-default-tab="html,result" data-slug-hash="YzrvENp" data-user="bryce-robinson"  data-prefill='{"tags":[],"scripts":[],"stylesheets":[]}'>
  <pre data-lang="html">&lt;div class="a">Box A min()&lt;/div>
&lt;div class="b">Box B max()&lt;/div>
&lt;div class="c">Box C clamp()&lt;/div>
</pre>
  <pre data-lang="css">div{
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  margin: 10px;
}
.a{
  width: min(10vw, 500px);
  height: min(10vw, 500px);
  background-color: red;
}

.b{
  width: max(10vw, 500px);
  height: max(10vw, 500px);
  background-color: blue;
}

.c{
  width: clamp(500px, 10vw, 1200px);
  height: clamp(500px, 10vw, 1200px);
  background-color:  green;
  
}</pre></div>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


```

---

### CSS min()
*example*
```
width: min(50vw, 500px)

```

This means the width of the div will be up to 500px, however, if the div is smaller than 50% of the VW, it will take up 50vw.

### CSS max()
*example*
```
width: max(50vw, 500px)

```
The minimum the div will be is 500px, or 50vw depending on which one is larger.

---

### CSS clamp()
*example*
```
width: clamp(500px, 10vw, 1200px)

```

syntax:
clamp(minimum value, preferred-value, max-value)

The preferred value will be used as long as it's within the min and max values.

---

*References*
[Clamp()](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp());

[Bits and pieces](https://blog.bitsrc.io/css-clamp-the-responsive-combination-weve-all-been-waiting-for-f1ce1981ea6e)
