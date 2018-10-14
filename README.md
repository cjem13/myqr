
## QR Code scanner for login hotspot MikroTik

### 

1. Add a button at login.html
```
<button onclick="window.location='https://cjem13.github.io/myqr';">QR Code</button>
```
2. Add the following script in MikroTik via Terminal.
```
/ip hotspot walled-garden ip

add action=accept comment="B-HOTSPOT QR Code Scanner" disabled=no dst-host=cjem13.github.io
```

### Powered by JEM.