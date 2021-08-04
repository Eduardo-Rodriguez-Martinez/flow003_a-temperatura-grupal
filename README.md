# flow003_a-temperatura-grupal
 Tarea que integra MQTT y Node-RED

 El commit inicial envia una temperatura fija.

 En el segundo commit se añadio la función para generar un numero aleatorio entre 20 y 10 para transmitirlo como temperatura.

 La funcion es
```Java
var mydate = new Date(msg.payload);
var mytemp = Math.floor((Math.random() * 20) + 10);
msg.payload = '{"ID":"Eduardo Rodriguez Martinez","Temp":"'+mytemp.toString()+'","mnsg":"'+mydate.toString()+'"}';
return msg;
```
