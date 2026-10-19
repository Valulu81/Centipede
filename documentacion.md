# 1 Aplicación o mini-juego funcional
## 1.1 Enlace a repositorio:
https://github.com/Valulu81/Centipede.git
## 1.2 Enlace a Despliegue en Netlify:
https://centipede-project.netlify.app/

# 2 Evidencia de vibecoding (prompts)
## 2.1 Prompts utilizados:

> <small>Eres un experto en la elaboración de videojuegos con Python y JavaScript, especializado en optimización y código limpio. tu objetivo es generar una solución eficiente.</small>
> <small>Crea el juego antiguo Centipede que sea funcional, diciéndome que librerías o elementos se usarían para su creación, debe de constar con 2 niveles según el juego, para mayor contexto, es de disparar a una serpiente, si es en la cabeza reduce su tamaño, pero si es en el cuerpo este se divide, en el mapa hay varios hongos que sirven para que el enemigo no sea disparado consecutivamente, y que se pueden ir destruyendo poco a poco, con el tiempo pasas de nivel y el enemigo es ligeramente más rápido.</small>
> <small>Necesito todo el código y herramientas necesarias, puedes hacerlo en js o Python.</small>
> <small>La solución debe de ser funcional e interactuable, puedes agregar elementos que enriquezcan la experiencia si yo lo apruebo</small>

> <small>Actúa como desarrollador experto. Estamos mejorando un clon del juego Centipede. Implementa los siguientes cambios en el código existente:</small>
> <small>1. Enemigos y Mecánicas:</small>
> <small>2. Añade "Arañas" y "Pulgas" como nuevos enemigos. Ambos deben tener 1 HP (mueren de 1 disparo).</small>
> <small>Valeria Liseth Paredes Lara</small>
> <small>3. Arañas: Movimiento en zig-zag en la parte inferior de la pantalla.</small>
> <small>4. Pulgas: Caída vertical rápida, dejando hongos a su paso.</small>
> <small>5. Diseño Visual (Sprites/Dibujo):</small>
> <small>6. Ciempiés/Serpiente: Modifica la función de renderizado para que cada segmento tenga 2 pares de patas animadas y la cabeza incluya una boca y ojos.</small>
> <small>7. Arañas/Pulgas: Genera un diseño pixel-art básico en base64 o funciones de dibujo de polígonos que las haga fácilmente identificables.</small>
> <small>8. Sonido (Web Audio API / Biblioteca nativa):</small>
> <small>9. Implementa efectos de sonido cortos para: Disparo del jugador y Movimiento del ciempiés.</small>
> <small>10. Añade una pista de música chiptune retro en bucle para el fondo.</small>
> <small>11. Sistema de Niveles (Total: 5 niveles):</small>
> <small>12. Transición: Avanzar de nivel cambia el color de fondo y de los enemigos. Los enemigos y hongos de la zona inferior comparten la misma paleta que el nivel para camuflarse.</small>
> <small>13. Nivel 1 (Verde): Dificultad base. Solo ciempiés.</small>
> <small>14. Nivel 2 (Morado): Aumenta velocidad base un 15%. Introduce Arañas.</small>
> <small>15. Nivel 3 (Rojo): Aumenta velocidad un 15% más. Introduce Pulgas (spawn cada 5 segundos).</small>
> <small>16. Nivel 4 (Amarillo): Aumenta velocidad de todos los enemigos y reduce el cooldown de disparo.</small>
> <small>17. Nivel 5 (Azul): Spawn rate de Arañas y Pulgas al máximo.</small>
> <small>18. Interfaz y Entorno:</small>
> <small>Valeria Liseth Paredes Lara</small>
> <small>19. Elimina la separación visual entre la zona del jugador (nave) y el resto del tablero. La nave debe moverse sobre el mismo fondo coloreado, y pueden aparecer hongos y arañas en su área de movimiento.</small>

> <small>Implementa las siguientes mejoras visuales y de interfaz en el código del juego:</small>
> <small>1. Diseño Responsivo y Controles Móviles:</small>
> <small>2. Adapta el canvas/contenedor para que sea responsive manteniendo su relación de aspecto (aspect ratio).</small>
> <small>3. Implementa una interfaz de controles táctiles (botones de flechas o joystick virtual) superpuesta mediante HTML/CSS.</small>
> <small>4. Utiliza CSS Media Queries (ej. @media (pointer: coarse)) para asegurar que estos controles táctiles se muestren *exclusivamente* en dispositivos móviles, permaneciendo ocultos en la versión de escritorio (donde se usa WASD).</small>
> <small>5. Persistencia de Puntaje Máximo (High Score):</small>
> <small>6. Modifica la UI para mostrar el "Puntaje Máximo" junto al puntaje actual.</small>
> <small>7. Implementa localStorage para guardar, actualizar y recuperar el puntaje máximo para que persista al recargar el navegador.</small>
> <small>8. Estilo de Fondo (Desktop):</small>
> <small>9. Añade un fondo personalizado (imagen, patrón geométrico o gradiente CSS estilo retro) al body o contenedor principal, de modo que el canvas del juego quede centrado y enmarcado en pantallas grandes.</small>
> <small>10. Aplica un box-shadow o borde al canvas para separarlo visualmente del nuevo fondo.</small>

## 2.2 Explicación de que se le pidió y que se mejoro
En los promps procure ir de lo más básico a más detalles, por lo cual en el primer prompt me dio un prototipo funcional que cumplía con lo solicitado, para los siguientes promps mejore detalles, como lo visual (arreglando el diseño de los enemigos), el sonido (con música, disparo y movimiento), la forma de interactuar (para pc y móvil); para que el juego fuera mas inmersivo y completo.
Mis prompt originales eran un poco mas robustos, pero con ayuda de otra IA (Gemini), pude darle un refinamiento adecuado para que Claude entendiera que es lo que estaba pidiendo y el como llevarlo a cabo, aunque siempre respetando la estructura de prompt dada en clases.

# 3 Iteración y mejora
Como se menciono anteriormente, el proyecto fue de menos a más, empezando con algo básico. El primer prompt fue solo para darle vida al proyecto.
En el segundo; se solicitó a la IA el que cambiara el diseño de los enemigos, puesto que eran muy simples (círculos solidos), y que agregara una ambientación, agregando música, sonido de disparos y el arrastre de enemigos; por último, que el escenario cambiara según nivel, siendo que el color principal y la dificultad varía según nivel. Aquí también se pidió el agregar mas enemigos para que fuera mas similar al juego original.
Por último, en el tercer promp se arreglaron cosas generales, como el fondo, para que no se viera tan vacío, además de hacer que fuera una interfaz interactiva tanto como para móviles como para escritorios, asegurando que en móviles se tuvieran los botones necesarios para poder jugar sin problemas.

# 4 Validación del resultado
## 4.1 ¿Cómo se probó el código?
Claude permite mostrar una preview de lo realizado, ahí pude jugar el proyecto en cada versión y ver que cosas se podían mejorar y que se podría agregar.
## 4.2 Errores y ajustes realizados
Como tal no hubo errores, simplemente cosas a mejorar, como podría ser que en la primera versión se dejo un espacio para que la nave se moviera, este era gris y vacío, haciendo menos inmersiva la experiencia, eso se mejoró, haciéndolo del mismo color que lo demás y que se generen enemigos y hongos en esa zona.

# 5 Reflexión Final
Esta fue una experiencia en verdad divertida, nunca había hecho algo similar, por lo cual aproveche y cree un juego que me gustaba mucho; aprendí mucho, ya que con la nueva forma de crear prompt se nota que lo que se solicita y da la IA es mucho mas completo y acertado, confirmándolo en que me tomo solo 3 prompts el completar el proyecto, antes de estas enseñanzas hubiera tomado mucho más tiempo y tokens. El vibecoding supone una gran ventaja en proyectos como estos, donde simples instrucciones logran crear proyectos simples en su totalidad, que se pueden ir refinando poco a poco. El código es algo complicado de entender a primeras, porque crea desde cero todo, pero al prestar atención a cada función se puede entender que hace cada parte, y en el proceso aprendí cosas que no sabia de JavaScript.