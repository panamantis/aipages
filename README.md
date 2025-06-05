# aipages

Add this bookmarklet to your bookmarks bar to [describe what it does].

1. Select the code below by clicking and dragging over it:
   ```javascript
   javascript:(function(){alert('Hello from your bookmarklet!');})();


2
[Bookmarklet](javascript:void%20function%28%29%7Balert%28%22Test%22%29%7D%28%29%3B)  

3
html
<a href="javascript:void%20function%28%29{alert%28%22Hello%22%29}%28%29;">Drag Me</a>  

4

	``` `javascript:(function(){alert('Hi!')})();` ```

 5
 	`javascript:(()=>{alert('Hi')})();`

  


## 1 Single-line fenced code

```javascript
javascript:(function(){alert('Hello from single-line bookmarklet!')})();
```

---

## 2 Multiline fenced block (drag selection)

```javascript
javascript:(function(){
  alert('Hello from multiline bookmarklet!');
})();
```

---

## 3 Inline back-tick

Drag-select or double-click, then drag:  
`javascript:(()=>{alert('Hello from inline!')})();`

---

## 4 URL-encoded (parens/quotes escaped)

```javascript
javascript:void%20function%20()%7Balert('Hello%20URL-encoded')%7D();
```

---

## 5 Raw HTML anchor (plain)

```html
<a href="javascript:(function(){alert('Hi from anchor!')})();">
  Drag Me
</a>
```

---

## 6 Raw HTML anchor (URL-encoded)

```html
<a href="javascript:void%20function%28%29%7Balert%28'Hi%20encoded!'%29%7D%28%29;">
  Drag Me (Encoded)
</a>
```

---

## 7 Anchor styled as a button

```html
<style>
.bm-btn{padding:6px 10px;border:1px solid #777;border-radius:4px;background:#fafafa;}
</style>

<a class="bm-btn"
   href="javascript:(function(){alert('Styled button');})();">
  ➕ Bookmarklet
</a>
```

---

## 8 HTML-entity encoding for parens

```html
<a href="javascript:(function(){alert(&quot;Entity&nbsp;Hi&quot;)}&lpar;&rpar;);">
  Drag (&amp;lpar;&amp;rpar;)
</a>
```

---

## 9 Base-64 self-decoding

```javascript
javascript:(function(){eval(atob('YWxlcnQoIkJhc2U2NCBIZWxsbyEiKTs='));})();
```

---

## 10 Windows .url shortcut (copy into a file, save as `Tool.url`, then drag file)

```ini
[InternetShortcut]
URL=javascript:(function(){alert('Windows shortcut');})();
```

---

## 11 Eval-concat trick (dodges literal “javascript:” scanners)

```javascript
javascript:/*@*/(0,eval)("alert('Eval-concat Hi!')");
```

---

## 12 Code block with manual prefix (tell users to copy after “javascript:”)

```javascript
javascript:
(function(){
  alert('Manual-prefix Hi!');
})();
```

---
