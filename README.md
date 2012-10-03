Introduccion
Este proyecto consiste en la construcción de un programa, que despliega el contenido de un archivo PGN. 
PGN es la Notación portátil de juego (Del original en inglés: Portable Game Notation (.PGN)) es un formato 
de computadora para grabar partidas de ajedrez, tanto los movimientos como la información relacionada; la mayoría 
de los programas de ajedrez para computadora reconocen este formato que es muy popular como consecuencia de su 
fácil uso.

Descripción del contenido
El pgn contiene información sobre la partida y los pasos que se van dando en un juego de ajedrez

Tabla de significados
K  Rey
Q	Dama
R	Torre
B	Alfil
N	Caballo
“”	Peón (usualmente no se menciona)
x	Captura
O-O   O-O-O	Enroque
"+"	Jaque
"#"	Jaque Mate
(columna)(fila)	Posición (ejemplo: e4)

Por lo general el peón no es especificado, sin embargo, por formalidad se puede utilizar la letra 
mayúscula “P”. Existen variaciones de este lenguaje pues en algunas ocasiones los movimientos 
quedan ambiguos a la hora de escribirlos, entonces se utiliza el origen y el destino, a diferencia 
de solo el destino.

Definición de estructuras
Principalmente se utilizan arrays de elementos textuales ordenados lógicamente para mostrarlos según el jugador y 
el turno.

Compilación, ejecución y utilización
Se compila y ejecuta como cualquier otra aplicación en XUL.
Para utilizar el software se debe primero cargar un archivo PGN, posteriormente se navega a través de los 
turnos por medio de dos botones de navegación (atrás y adelante), se mostrarán los movimientos correspondientes 
para el jugador Blanco y el jugador de las piezas Negras.

Ejemplos
Ejemplo de PGN:
[Event "Wch U16"]
[Site "Wattignies"]
[Date "1976.??.??"]
[Round "?"]
[White "Chandler, Murray G"]
[Black "Kasparov, Garry"]
[Result "1-0"]
[ECO "B22"]
[PlyCount "82"]
[EventDate "1976.??.??"]

1.e4 c5 2.c3 Nf6 3.e5 Nd5 4.d4 Nc6 5.Nf3 cxd4 6.cxd4 e6 7.a3 d6 8.Bd3 Qa5+ 9.Bd2 Qb6 10.Nc3 Nxc3 11.Bxc3 dxe5 12.dxe5 Be7 13.O-O Bd7 14.Nd2 Qc7 15.Qg4 O-O-O 16.Rfc1 Kb8 17.Qc4 Rc8 18.b4 f6 19.Nf3 Qb6 20.Qe4 f5 21.Qe1 a6 22.Rab1 g5 23.Nd2 Nd4 24.Qe3 Rxc3 25.Rxc3 f4 26.Qe1 g4 27.Ne4 Bc6 28.Nc5 Ka7 29.a4 Bf3 30.a5 Qd8 31.Bc4 Bxc5 32.bxc5 Qh4 33.gxf3 gxf3 34.Kh1 Rg8 35.Qe4 Rg7 36.Qxd4 Qg5 37.c6+ Kb8 38.c7+ Rxc7 39.Rg1 Qh5 40.Rg8+ Rc8 41.Qd6+ Ka7  1-0



Limitaciones y mejoras
Entre las limitaciones encontradas se puede resaltar que estos archivos no contienen la 
información de el punto de salida de una ficha a el punto de llegada, por lo que depende de un 
contexto actual y una deducción lógica de cuál ficha puede hacer el movimiento si es que esta existe. 
Esto se podría hacer mediante complejos algoritmos que abarquen todos los comportamientos y posibles 
movimientos de las piezas del ajedrez por lo que consideramos que esto se encuentra fuera de las 
especificaciones del proyecto. También se consideran posibles mejoras agregando imágenes para representar 
cada pieza.
Cabe también mencionar como una limitante al contenido de los archivos, pues algunos PGN poseen más de una 
partida, ademas de caracteres ocultos como “\t” “\n”.