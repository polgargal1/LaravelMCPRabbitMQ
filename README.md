# Mi Proyecto Laravel MCP 
En esta práctica he montado un sistema para que mi aplicación de Laravel sea más inteligente y rápida usando herramientas modernas. Aquí explico paso a paso lo que he hecho:

1. ¿Qué he montado exactamente?
Básicamente, he hecho que tres cosas que no se conocían hablen entre sí:

Laravel: Que es el corazón de mi web.

RabbitMQ: Es como un "mensajero". Si la web tiene que hacer algo pesado (como enviar 1000 emails), se lo pide a RabbitMQ para no quedarse colgada. RabbitMQ los guarda en una lista y los va haciendo poco a poco.

Claude (IA): He configurado la aplicación de Claude para que pueda "ver" mi código de GitHub y ayudarme a programar mejor.

2. ¿Cómo lo he hecho? (Paso a paso)
El mensajero (Docker y RabbitMQ):
Instalé un programa que se llama Docker. Imagina que Docker es como un barco que lleva cajas. Dentro de una de esas cajas metí a RabbitMQ. Así, el "mensajero" está siempre listo en mi ordenador sin molestar a otros programas.

Conectar la IA con mi código (MCP):
Esto fue lo más guapo. Entré en los archivos secretos de configuración de Claude y le puse una "llave" (un Token) de mi GitHub. Gracias a esto, ahora Claude puede leer mi repositorio y sabe exactamente qué archivos tengo y qué errores hay.

Subir todo a GitHub:
Usé comandos de terminal (git push) para enviar mi trabajo a internet. Así, tanto mi profesor como la IA pueden ver lo que he programado.

3. ¿Para qué sirve?
La idea es que la web no se bloquee. Si un usuario hace clic en un botón, no tiene que esperar 10 segundos a que cargue todo. El mensaje se va a la "caja" de RabbitMQ y la web sigue funcionando rápido. Además, tener a la IA conectada me ayuda a encontrar fallos mucho más rápido.
