# Aron Isael Sánchez

Estudiante de ciberseguridad y TI. Diseño y dirijo software con IA: especifico, apruebo cada plan y verifico los resultados.

## Proyecto destacado: The IT.EXE

> *Antes llamado **The Mopris Castle**.* Repositorio privado por ahora.

Un RPG de acción 2D, hecho para **aprender TI jugando**. El mundo es la aldea de Mopris, que se recorre vista desde arriba como un RPG clásico: una casa por cada área de TI y, en medio, el castillo, que es la carrera (8 pisos = 8 semestres). Al cruzar una puerta, los niveles se juegan de lado, con salto y plataformas. Los enemigos son lo que complica una carrera de TI: bugs, exámenes sorpresa, fechas límite, un troyano disfrazado de café.

**Qué hay hoy** (el proyecto está en ampliación; lo que no existe aún no se cuenta):

| | |
|---|---|
| Contenido | 6 héroes, 21 enemigos, 5 jefes, 14 optativas |
| Aprendizaje | Temario con 23 fichas de TI y 21 certificaciones por rama (algunas, todavía «en obra») |
| Niveles | El castillo completo (8 niveles); 6 zonas más en construcción |
| Controles | Teclado y mouse, control (Xbox, PlayStation, Switch) y pantalla táctil, con íconos que cambian según el dispositivo |
| Sin archivos de arte ni audio | Los sprites se dibujan por código y el sonido se sintetiza con WebAudio |

**Origen.** La primera versión, *The Mopris Castle 2D*, se presentó en Expolitec 2026 como proyecto de equipo en la Escuela Politécnica de Guadalajara (UDG). Fui autor de la lógica del juego y de la documentación (ERS, manual técnico y manual de usuario, tomando como guía el estándar IEEE 830). *The IT.EXE* es su versión ampliada.

## Cómo trabajo con IA

No lo hago a ojo: el proyecto tiene un proceso escrito y comprobable.

- **Contexto como código.** Un `CLAUDE.md` con las reglas del proyecto, la lista de «trampas conocidas» y el mapa de archivos; un `PROGRESS.md` que se actualiza en cada tarea y es lo primero que se lee al retomar; y un protocolo propio para `/compact` y `/clear`, para no perder el hilo entre sesiones.
- **Diseño → plan → aprobación → código.** Cada tarea tiene su documento de diseño y su plan, y nada se construye hasta que yo los apruebo.
- **División de roles entre modelos.** Un modelo planifica y revisa, otro escribe el código a partir del plan y otro mantiene la documentación. La implementación la hacen agentes de IA; las decisiones de diseño y la aprobación son mías.
- **Una rama de git por tarea**, integrada a `master` solo al cerrarla, para que el juego siempre se pueda jugar.
- **Pruebas automáticas** en un navegador sin ventana, con casos que miden, por ejemplo, que el HUD tape como máximo el 8 % de la pantalla.

## Seguridad en el diseño

Reglas del proyecto, escritas de antemano: el guardado local se trata como entrada no confiable y se valida al leerlo; el texto del usuario se pinta con `textContent`, nunca con `innerHTML`; y la clave `service_role` de Supabase no va en el cliente.

## Stack

`JavaScript` · `HTML` · `CSS` · `Phaser 3` · `WebAudio` · `Gamepad API` · `Git` · `Supabase (diseño del ranking en línea, sin desplegar)`

## Contacto

Aquí, en GitHub: [@Isael1x1](https://github.com/Isael1x1)
