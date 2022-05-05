# java-full-stack-dev-u17

Este repositorio corresponde a ejercicios realizados en la formación de Java Full Stack Developer, concretamente a la unidad 17 UD17 – MongoDB

#Ejercicio 1

```
use ejercicio1
db.createCollection("fabricantes")
db.fabricantes.insertOne({codigo:1,nombre:"Asus"})
db.fabricantes.insertOne({codigo:2,nombre:"Acer"})
db.fabricantes.insertOne({codigo:3,nombre:"Apple"})
db.fabricantes.insertOne({codigo:4,nombre:"Sony"})
db.fabricantes.insertOne({codigo:5,nombre:"Lenovo"})
db.fabricantes.insertOne({codigo:6,nombre:"Dell"})
db.fabricantes.insertOne({codigo:7,nombre:"Fujitsu"})
db.fabricantes.insertOne({codigo:8,nombre:"HP"})
db.fabricantes.insertOne({codigo:9,nombre:"Chromebooks"})
db.fabricantes.insertOne({codigo:10,nombre:"Samsung"})
db.fabricantes.find()
db.createCollection("articulos")
db.articulos.insertOne({codigo:1,nombre:"Portatil 1",precio:1021,fabricante:1})
db.articulos.insertOne({codigo:2,nombre:"Portatil 2",precio:1022,fabricante:2})
db.articulos.insertOne({codigo:3,nombre:"Portatil 3",precio:1023,fabricante:3})
db.articulos.insertOne({codigo:4,nombre:"Portatil 4",precio:1024,fabricante:4})
db.articulos.insertOne({codigo:5,nombre:"Portatil 5",precio:1026,fabricante:5})
db.articulos.insertOne({codigo:6,nombre:"Portatil 6",precio:1026,fabricante:6})
db.articulos.insertOne({codigo:7,nombre:"Portatil 7",precio:1027,fabricante:7})
db.articulos.insertOne({codigo:8,nombre:"Portatil 8",precio:1028,fabricante:8})
db.articulos.insertOne({codigo:9,nombre:"Portatil 9",precio:1029,fabricante:9})
db.articulos.insertOne({codigo:10,nombre:"Portatil 10",precio:1030,fabricante:10})
db.articulos.find()
```

#Ejercicio2 

```
use ejercicio2
db.createCollection("departamentos")
db.departamentos.insertOne({codigo:1,nombre:"Ventas",presupuesto:103000})
db.departamentos.insertOne({codigo:2,nombre:"Investigación",presupuesto:140000})
db.departamentos.insertOne({codigo:3,nombre:"Administración",presupuesto:200000})
db.departamentos.insertOne({codigo:4,nombre:"Innovación",presupuesto:670000})
db.departamentos.insertOne({codigo:5,nombre:"Desarrollo",presupuesto:23000})
db.departamentos.insertOne({codigo:6,nombre:"Diseño",presupuesto:560000})
db.departamentos.insertOne({codigo:7,nombre:"Marketing",presupuesto:190000})
db.departamentos.insertOne({codigo:8,nombre:"Dirección",presupuesto:500000})
db.departamentos.insertOne({codigo:9,nombre:"Ejecutivos intermedios",presupuesto:900000})
db.departamentos.insertOne({codigo:10,nombre:"Altos Ejecutivos",presupuesto:9000000})
db.departamentos.find()
db.createCollection("empleados")
db.empleados.insertOne({DNI:1,nombre:"Empleado 1",apellidos:"Apellido empleado 1",departamento:1})
db.empleados.insertOne({DNI:2,nombre:"Empleado 2",apellidos:"Apellido empleado 2",departamento:2})
db.empleados.insertOne({DNI:3,nombre:"Empleado 3",apellidos:"Apellido empleado 3",departamento:3})
db.empleados.insertOne({DNI:4,nombre:"Empleado 4",apellidos:"Apellido empleado 4",departamento:4})
db.empleados.insertOne({DNI:5,nombre:"Empleado 5",apellidos:"Apellido empleado 5",departamento:5})
db.empleados.insertOne({DNI:6,nombre:"Empleado 6",apellidos:"Apellido empleado 6",departamento:6})
db.empleados.insertOne({DNI:7,nombre:"Empleado 7",apellidos:"Apellido empleado 7",departamento:7})
db.empleados.insertOne({DNI:8,nombre:"Empleado 8",apellidos:"Apellido empleado 8",departamento:8})
db.empleados.insertOne({DNI:9,nombre:"Empleado 9",apellidos:"Apellido empleado 9",departamento:9})
db.empleados.insertOne({DNI:10,nombre:"Empleado 10",apellidos:"Apellido empleado 10",departamento:10})
db.empleados.find()
```

#Ejercicio 3

```
use ejercicio3
db.createCollection("cajas")
db.cajas.insertOne({numReferencia:"0MN7",contenido:"Rocks",valor:103,almacen:1})
db.cajas.insertOne({numReferencia:"4H8P",contenido:"Rocks",valor:140,almacen:2})
db.cajas.insertOne({numReferencia:"4RT3",contenido:"Scissors",valor:200,almacen:3})
db.cajas.insertOne({numReferencia:"7G3H",contenido:"Rocks",valor:670,almacen:4})
db.cajas.insertOne({numReferencia:"8JN6",contenido:"Papers",valor:23,almacen:5})
db.cajas.insertOne({numReferencia:"8Y6U",contenido:"Papers",valor:560,almacen:6})
db.cajas.insertOne({numReferencia:"9J6F",contenido:"Papers",valor:190,almacen:7})
db.cajas.insertOne({numReferencia:"LL08",contenido:"Rocks",valor:500,almacen:8})
db.cajas.insertOne({numReferencia:"P0H6",contenido:"Scissors",valor:90,almacen:9})
db.cajas.insertOne({numReferencia:"P2T6",contenido:"Scissors",valor:90,almacen:10})
db.cajas.find()
db.createCollection("almacenes")
db.almacenes.insertOne({codigo:1,lugar:"Ventas",capacidad:1030})
db.almacenes.insertOne({codigo:2,lugar:"Investigación",capacidad:1400})
db.almacenes.insertOne({codigo:3,lugar:"Administración",capacidad:2000})
db.almacenes.insertOne({codigo:4,lugar:"Innovación",capacidad:6700})
db.almacenes.insertOne({codigo:5,lugar:"Desarrollo",capacidad:200})
db.almacenes.insertOne({codigo:6,lugar:"Diseño",capacidad:5000})
db.almacenes.insertOne({codigo:7,lugar:"Marketing",capacidad:1900})
db.almacenes.insertOne({codigo:8,lugar:"Dirección",capacidad:5000})
db.almacenes.insertOne({codigo:9,lugar:"Ejecutivos intermedios",capacidad:9000})
db.almacenes.insertOne({codigo:10,lugar:"Altos Ejecutivos",capacidad:90000})
db.almacenes.find()
db.almacenes.replaceOne({"_id":ObjectId("627426466000e90e23913441")}, {"codigo": 1,  "lugar": "Valencia",  "capacidad": 1030})
db.almacenes.replaceOne({"_id":ObjectId("627426466000e90e23913442")}, {"codigo": 2,  "lugar": "Barcelona",  "capacidad": 1400})
db.almacenes.replaceOne({"_id":ObjectId("627426466000e90e23913443")}, {"codigo": 3,  "lugar": "Valencia",  "capacidad": 2000})
db.almacenes.replaceOne({"_id":ObjectId("627426466000e90e23913444")}, {"codigo": 4,  "lugar": "Bilbao",  "capacidad": 6700})
db.almacenes.replaceOne({"_id":ObjectId("627426466000e90e23913445")}, {"codigo": 5,  "lugar": "Los Angeles",  "capacidad": 200})
db.almacenes.replaceOne({"_id":ObjectId("627426466000e90e23913446")}, {"codigo": 6,  "lugar": "San Francisco",  "capacidad": 5000})
db.almacenes.replaceOne({"_id":ObjectId("627426466000e90e23913447")}, {"codigo": 7,  "lugar": "Valencia",  "capacidad": 1900})
db.almacenes.replaceOne({"_id":ObjectId("627426466000e90e23913448")}, {"codigo": 8,  "lugar": "Barcelona",  "capacidad": 5000})
db.almacenes.replaceOne({"_id":ObjectId("627426466000e90e2391344a")}, {"codigo": 10,  "lugar": "Bilbao",  "capacidad": 90000})
db.almacenes.replaceOne({"_id":ObjectId("627426466000e90e23913449")}, {"codigo": 9,  "lugar": "Barcelona",  "capacidad": 9000})
```

#Ejercicio 4 

```
use ejercicio4
db.createCollection("salas")
db.salas.insertOne({codigo:1,nombre:"Sala J",pelicula:10})
db.salas.insertOne({codigo:2,nombre:"Sala I",pelicula:1})
db.salas.insertOne({codigo:3,nombre:"Sala H",pelicula:2})
db.salas.insertOne({codigo:4,nombre:"Sala G",pelicula:3})
db.salas.insertOne({codigo:5,nombre:"Sala F",pelicula:4})
db.salas.insertOne({codigo:6,nombre:"Sala E",pelicula:5})
db.salas.insertOne({codigo:7,nombre:"Sala D",pelicula:6})
db.salas.insertOne({codigo:8,nombre:"Sala C",pelicula:7})
db.salas.insertOne({codigo:9,nombre:"Sala B",pelicula:8})
db.salas.insertOne({codigo:10,nombre:"Sala A",pelicula:9})
db.salas.find()
db.createCollection("peliculas")
db.peliculas.insertOne({codigo:1,nombre:"Citizen Kane",calificacionEdad:10})
db.peliculas.insertOne({codigo:2,nombre:"Singin\' in the Rain",calificacionEdad:14})
db.peliculas.insertOne({codigo:3,nombre:"The Wizard of Oz",calificacionEdad:18})
db.peliculas.insertOne({codigo:4,nombre:"The Quiet Man",calificacionEdad:6})
db.peliculas.insertOne({codigo:5,nombre:"North by Northwest",calificacionEdad:2})
db.peliculas.insertOne({codigo:6,nombre:"The Last Tango in Paris",calificacionEdad:5})
db.peliculas.insertOne({codigo:7,nombre:"A Night at the Opera",calificacionEdad:18})
db.peliculas.insertOne({codigo:8,nombre:"Citizen King",calificacionEdad:5})
db.peliculas.insertOne({codigo:9,nombre:"Hasta el último hombre",calificacionEdad:9})
db.peliculas.insertOne({codigo:10,nombre:"Matrix",calificacionEdad:9})
db.peliculas.find()
```

#Ejercicio 5

```
use ejercicio5
db.createCollection("despachos")
db.despachos.insertOne({numero:1,capacidad:10})
db.despachos.insertOne({numero:2,capacidad:10})
db.despachos.insertOne({numero:3,capacidad:20})
db.despachos.insertOne({numero:4,capacidad:30})
db.despachos.insertOne({numero:5,capacidad:40})
db.despachos.insertOne({numero:6,capacidad:50})
db.despachos.insertOne({numero:7,capacidad:60})
db.despachos.insertOne({numero:8,capacidad:70})
db.despachos.insertOne({numero:9,capacidad:80})
db.despachos.insertOne({numero:10,capacidad:90})
db.despachos.find()
db.createCollection("directores")
db.directores.insertOne({DNI:"123234877",nombreCompleto:"Michael Rogers",despacho:10,DNIjefe: null})
db.directores.insertOne({DNI:"152934485",nombreCompleto:"Anand Manikutty",despacho:14,DNIjefe: null})
db.directores.insertOne({DNI:"222364883",nombreCompleto:"Carol Smith",despacho:18,DNIjefe:"123234877"})
db.directores.insertOne({DNI:"326587417",nombreCompleto:"Joe Man",despacho:6,DNIjefe: null})
db.directores.insertOne({DNI:"332154719",nombreCompleto:"Stevens Northwest",despacho:2,DNIjefe:null})
db.directores.insertOne({DNI:"332569843",nombreCompleto:"Mary-Anne Paris",despacho:5,DNIjefe:"326587417"})
db.directores.insertOne({DNI:"546523478",nombreCompleto:"Foster Opera",despacho:18,DNIjefe:"326587417"})
db.directores.insertOne({DNI:"631231482",nombreCompleto:"George King",despacho:5,DNIjefe:"326587417"})
db.directores.insertOne({DNI:"654873219",nombreCompleto:"John Doe",despacho:9,DNIjefe:"546523478"})
db.directores.insertOne({DNI:"745685214",nombreCompleto:"David Smith",despacho:9,DNIjefe:null})
db.directores.find()
```

#Ejercicio 6 

```
use ejercicio6
db.createCollection("piezas")
db.piezas.insertOne({codigo:1,nombre:"Batería"})
db.piezas.insertOne({codigo:2,nombre:"Bombillas"})
db.piezas.insertOne({codigo:3,nombre:"Discos de frenos"})
db.piezas.insertOne({codigo:4,nombre:"Parabrisas"})
db.piezas.insertOne({codigo:5,nombre:"Indicador de presión de neumáticos"})
db.piezas.insertOne({codigo:6,nombre:"Faros delanteros"})
db.piezas.insertOne({codigo:7,nombre:"Bujías"})
db.piezas.insertOne({codigo:8,nombre:"Mando de llave a distancia"})
db.piezas.insertOne({codigo:9,nombre:"Tiradores de puertas y seguros de cierre"})
db.piezas.insertOne({codigo:10,nombre:"Fusibles"})
db.piezas.find()
db.createCollection("proveedores")
db.proveedores.insertOne({id:"000A",nombre:"Tiendas Aurgi"})
db.proveedores.insertOne({id:"000B",nombre:"Autoexpress"})
db.proveedores.insertOne({id:"000C",nombre:"Totcar"})
db.proveedores.insertOne({id:"000D",nombre:"Oscaro"})
db.proveedores.insertOne({id:"000E",nombre:"Recambios-expres"})
db.proveedores.insertOne({id:"000F",nombre:"Norauto"})
db.proveedores.insertOne({id:"000G",nombre:"Rexbo"})
db.proveedores.insertOne({id:"000H",nombre:"Piezascochesonline"})
db.proveedores.insertOne({id:"000I",nombre:"Dosochoauto"})
db.proveedores.insertOne({id:"000J",nombre:"Recambioclasico"})
db.proveedores.find()
db.createCollection("suministra")
db.suministra.insertOne({codigoPieza:"1",idProveedor:"000D",precio:10})
db.suministra.insertOne({codigoPieza:"2",idProveedor:"000A",precio:14})
db.suministra.insertOne({codigoPieza:"3",idProveedor:"000B",precio:18})
db.suministra.insertOne({codigoPieza:"4",idProveedor:"000E",precio:61})
db.suministra.insertOne({codigoPieza:"5",idProveedor:"000C",precio:28})
db.suministra.insertOne({codigoPieza:"6",idProveedor:"000G",precio:55})
db.suministra.insertOne({codigoPieza:"7",idProveedor:"000F",precio:18})
db.suministra.insertOne({codigoPieza:"8",idProveedor:"000J",precio:57})
db.suministra.insertOne({codigoPieza:"9",idProveedor:"000I",precio:97})
db.suministra.insertOne({codigoPieza:"10",idProveedor:"000H",precio:97})
db.suministra.find()
```

#Ejercicio 7

```
use ejercicio7
db.cajeros.insertMany([{codigo:"12345684",nombre_completo:'Jose González Ruiz'},
{codigo:"12345685",nombre_completo:'Daniel Fernandez Lujan'},
{codigo:"12345686",nombre_completo:'Joan Hurtado Martín'},
{codigo:"12345687",nombre_completo:'Miguel Alcántara Garrido'},
{codigo:"12345688",nombre_completo:'Gerard Martinez Soja'},
{codigo:"12345689",nombre_completo:'Marc Marquez Sevilla'},
{codigo:"12345610",nombre_completo:'Veronika Rexbo Tomico'},
{codigo:"12345611",nombre_completo:'Constant Tomico Rexbo'},
{codigo:"12345612",nombre_completo:'Octavi Herraiz Llull'},
{codigo:"12345613",nombre_completo:'Aida Queralt Lozano'},
{codigo:"12345696",nombre_completo:'Adria Ruiz Esteban'}])

db.productos.insertMany([{codigo:1,nombre:"Paneles solares y cargadores",precio:54},
{codigo:2,nombre:"Llaveros inteligentes",precio:45},
{codigo:3,nombre:"Altavoces portátiles",precio:23},
{codigo:4,nombre:"Termómetros para bebés",precio:98},
{codigo:5,nombre:"Asientos de automóvil",precio:57},
{codigo:6,nombre:"Cortaúñas para bebés",precio:22},
{codigo:7,nombre:"Camas para mascotas",precio:30},
{codigo:8,nombre:"Cuencos de alimentación personalizados",precio:54},
{codigo:9,nombre:"Collares de entrenamiento",precio:34},
{codigo:0,nombre:"Mochilas",precio:34}])

db.maquinaRegistradoras.insertMany([{codigo:1,piso:1},
{codigo:2,piso:2},
{codigo:3,piso:3},
{codigo:4,piso:4},
{codigo:5,piso:5},
{codigo:6,piso:6},
{codigo:7,piso:7},
{codigo:8,piso:8},
{codigo:9,piso:9},
{codigo:0,piso:0}])

db.venta.insertMany([{cajero:12345684,maquina:1,producto:7},
{cajero:12345688,maquina:3,producto:5},
{cajero:12345684,maquina:2,producto:4},
{cajero:12345688,maquina:5,producto:4},
{cajero:12345684,maquina:7,producto:4},
{cajero:12345688,maquina:9,producto:4},
{cajero:12345684,maquina:0,producto:4},
{cajero:12345684,maquina:8,producto:3},
{cajero:12345696,maquina:7,producto:2},
{cajero:12345688,maquina:1,producto:1}])
```

#Ejercicio 8

```
use ejercicio8
db.facultades.insertMany([{codigo:1,nombre:"UAB"},
{codigo:2,nombre:"URV"},
{codigo:3,nombre:"Hardvard"},
{codigo:4,nombre:"Candbridge"},
{codigo:5,nombre:"Universitat de Valencia"},
{codigo:6,nombre:"MIT"},
{codigo:7,nombre:"Cannes"},
{codigo:8,nombre:"UMAA"},
{codigo:9,nombre:"UTL Salke"},
{codigo:0,nombre:"Universida Granada"}])

db.investigadores.insertMany([{DNI:"12345684",nombreCompleto:"Jose González Ruiz",facultad:1},
{DNI:"12345685",nombreCompleto:"Daniel Fernandez Lujan",facultad:2},
{DNI:"12345686",nombreCompleto:"Joan Hurtado Martín",facultad:3},
{DNI:"12345687",nombreCompleto:"Miguel Alcántara Garrido",facultad:4},
{DNI:"12345688",nombreCompleto:"Gerard Martinez Soja",facultad:5},
{DNI:"12345689",nombreCompleto:"Marc Marquez Sevilla",facultad:6},
{DNI:"12345610",nombreCompleto:"Veronika Rexbo Tomico",facultad:7},
{DNI:"12345611",nombreCompleto:"Constant Tomico Rexbo",facultad:8},
{DNI:"12345612",nombreCompleto:"Octavi Herraiz Llull",facultad:9},
{DNI:"12345613",nombreCompleto:"Aida Queralt Lozano",facultad:0}])

db.equipos.insertMany([
{numeroSerie:"fase",nombre:"Equipo0",facultad:0},
{numeroSerie:"dfsd",nombre:"Equipo3",facultad:8},
{numeroSerie:"uER3",nombre:"Equipo4",facultad:7},
{numeroSerie:"Sdfa",nombre:"Equipo5",facultad:9},
{numeroSerie:"sdfe",nombre:"Equipo6",facultad:3},
{numeroSerie:"dfas",nombre:"Equipo5",facultad:7},
{numeroSerie:"JKds",nombre:"Equipo6",facultad:3},
{numeroSerie:"djdf",nombre:"Equipo1",facultad:2},
{numeroSerie:"dssd",nombre:"Equipo5",facultad:1},
{numeroSerie:"dass",nombre:"Equipo1",facultad:1}])

db.reserva.insertMany([
{DNI:"12345684",numeroSerie:"fase",comienzo: "2010-05-10",fin: "2010-06-10"},
{DNI:"12345686",numeroSerie:"dfsd",comienzo: "2010-05-23",fin: "2010-06-12"},
{DNI:"12345685",numeroSerie:"uER3",comienzo: "2010-05-23",fin: "2010-06-12"},
{DNI:"12345687",numeroSerie:"uER3",comienzo: "2010-05-23",fin: "2010-06-12"},
{DNI:"12345688",numeroSerie:"sdfe",comienzo: "2010-05-23",fin: "2010-06-12"},
{DNI:"12345689",numeroSerie:"dssd",comienzo: "2010-05-23",fin: "2010-06-12"},
{DNI:"12345610",numeroSerie:"JKds",comienzo: "2010-03-23",fin: "2010-06-12"},
{DNI:"12345611",numeroSerie:"JKds",comienzo: "2010-05-23",fin: "2010-06-12"},
{DNI:"12345612",numeroSerie:"Sdfa",comienzo: "2010-03-23",fin: "2010-06-12"},
{DNI:"12345613",numeroSerie:"dass",comienzo: "2010-05-23",fin: "2010-04-12"}])
```

#Ejercicio 9

```
use ejercicio9
db.cientificos.insertMany([
    {DNI:'12345684',nombreCompleto: 'Jose González Ruiz'},
    {DNI:'12345685',nombreCompleto: 'Daniel Fernandez Lujan'},
    {DNI:'12345686',nombreCompleto: 'Joan Hurtado Martín'},
    {DNI:'12345687',nombreCompleto: 'Miguel Alcántara Garrido'},
    {DNI:'12345688',nombreCompleto: 'Gerard Martinez Soja'},
    {DNI:'12345689',nombreCompleto: 'Marc Marquez Sevilla'},
    {DNI:'12345610',nombreCompleto: 'Veronika Rexbo Tomico'},
    {DNI:'12345611',nombreCompleto: 'Constant Tomico Rexbo'},
    {DNI:'12345612',nombreCompleto: 'Octavi Herraiz Llull'},
    {DNI:'12345613',nombreCompleto: 'Aida Queralt Lozano'}
])



db.proyectos.insertMany([
    {id:'0001' ,nombre: 'EL BILLETE QUE ARDE… ¡Y NO SE QUEMA!',hores:10},
{id:'0002' ,nombre: 'CAMINAR SOBRE HUEVOS… ¡SIN ROMPERLOS!',hores:50},
{id:'0003' ,nombre: 'VIENDO BAILAR A LAS ONDAS DE SONIDO',hores:60},
{id:'0004' ,nombre: 'HAZ GEODAS CON HUEVOS',hores:30},
{id:'0005' ,nombre: 'CONVERTIR UNA PASTILLA DE JABÓN DE MARFIL EN UNA PALOMITA MONSTRUOSA',hores:80},
{id:'0006' ,nombre: '¡LAS PLANTAS CAMBIAN DE COLOR!',hores:50},
{id:'0007' ,nombre: 'HACIENDO ENGORDAR A LOS OSITOS DE GOMA (Y OTRAS COSAS PEORES…)',hores:15},
{id:'0008' ,nombre: 'ROCK CANDY CASERO… ¡Y CON UN PALO!',hores:20},
{id:'0009' ,nombre: 'UNA PLANTA QUE CRECE EN UN CD',hores:12},
{id:'0010' ,nombre: 'AGUJEREAR LA BOLSA SIN QUE SE SALGA EL AGUA',hores: 4}
])



db.asignado_a.insertMany([
{cientifico:'12345684',proyecto:'0010',precio:20},
{cientifico:'12345685',proyecto:'0001',precio:10},
{cientifico:'12345686',proyecto:'0002',precio:24},
{cientifico:'12345687',proyecto:'0003',precio:30},
{cientifico:'12345688',proyecto:'0004',precio:10},
{cientifico:'12345689',proyecto:'0005',precio:20},
{cientifico:'12345610',proyecto:'0006',precio:24},
{cientifico:'12345611',proyecto:'0007',precio:22},
{cientifico:'12345612',proyecto:'0008',precio:68},
{cientifico:'12345613',proyecto:'0009',precio:50}
])
```
