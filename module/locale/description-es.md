# Smarter Patrols

**Autor**: Monsterfish
**Versión**: 1.0.1

Hace que las tropas de patrulla y escolta de asedio de la IA utilicen realmente todos sus grupos durante un ataque. Ambas partes pueden desactivarse en los ajustes.

## Tropas de patrulla

En el juego original solo el primer grupo de patrulla recibe órdenes. El segundo se queda parado en el punto de reunión durante todo el ataque.

Con este módulo, cada grupo de patrulla sigue su propia ruta alrededor del castillo atacado:

- **Grupo 1** rodea el castillo en un sentido.
- **Grupo 2** lo rodea en el sentido contrario.
- **Grupo 3** recorre de ida y vuelta el frente del castillo (el lado orientado hacia el atacante).
- **Grupos 4, 5 y 6** hacen lo mismo que 1, 2 y 3, pero un cuarto de vuelta por detrás; los grupos 7, 8 y 9 van detrás de ellos, y así sucesivamente.

Caminan a una distancia a pie fijada fuera del castillo (12 casillas por defecto, como la patrulla del juego), de modo que rodean muros y fosos en lugar de meterse en ellos. Si un grupo se encuentra con enemigos, lucha primero y después sigue su ruta.

## Tropas de escolta de asedio

Estas tropas ya caminan de una máquina de asedio a otra, pero ambos grupos hacen el mismo recorrido al mismo tiempo, por lo que actúan como un solo grupo.

Con este módulo:

- Cada grupo empieza junto a una máquina de asedio distinta y uno de cada dos camina en sentido contrario, cubriendo todas las máquinas.
- Los grupos compuestos sobre todo por unidades cuerpo a cuerpo avanzan unas casillas por delante de las máquinas (hacia el castillo) para atraer el fuego de los defensores en lugar de las máquinas. Los arqueros se quedan junto a las máquinas.
- Cuando empieza el asalto a los muros, todos los grupos atacan igual que en el juego original.

## Más grupos

El juego solo soporta 2 grupos de patrulla y 2 grupos de escolta de asedio. Si un archivo de IA pide más, las unidades sobrantes acaban en las tropas equivocadas (cavadores de foso o ejército principal). Este módulo permite hasta 12 de cada tipo. La cantidad procede del archivo de la IA salvo que indiques otra en los ajustes (escolta de asedio: 4 por defecto). Una tropa solo se divide mientras cada grupo conserve al menos 4 unidades (valor configurable).

Los grupos adicionales solo existen mientras el ejército está atacando. Al abrirse una brecha en el castillo, morir el señor o retirarse la IA, se reincorporan al resto y vuelven a seguir las órdenes habituales de la IA.

## Conviene saber

- Solo afecta a los ataques de la IA; tus propias tropas no cambian.
- Funciona junto con Lord Hunt.
- No se guarda ningún dato adicional en las partidas guardadas.
