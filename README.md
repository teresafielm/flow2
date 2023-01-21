# flow2

Este repositorio es para el flow2 que se hizo en Node-RED.

El presente código se implemento en el bloque funtion, cuyo proposito es mostrar el mes, día, año y hora junto a que región de horario estamos (GMT).

// Lo que está después de “//” son comentarios

// Crea un objeto Date a partir del payload enviado por timestamp

var date = new Date(msg.payload);

// Cambia el payload para que sea una fecha con formato

msg.payload = date.toString();

// Regresa el mensaje para que se envíe al sigueinte nodo

return msg;
