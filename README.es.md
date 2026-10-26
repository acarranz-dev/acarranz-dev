<div align="center">

# Andreu Carranza

**Programador en C, C++ y Python formado en 42 Barcelona. Diseño arquitecturas multiagente sobre LLM: descomposición de tareas, enrutado semántico y verificación cruzada entre agentes.**

[English](README.md) · [Català](README.ca.md) · **Español**

[![42 Barcelona](https://img.shields.io/badge/42-Barcelona-000000?style=for-the-badge&logo=42&logoColor=white)](https://www.42barcelona.com)
[![Ubicación](https://img.shields.io/badge/Cataluña-España-1f6feb?style=for-the-badge)](#)
[![Email](https://img.shields.io/badge/Email-contacto-ea4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:andreucarranzagibert@gmail.com)

</div>

---

## Sobre mí

Soy desarrollador formado en **42 Barcelona**, una escuela entre iguales sin
profesores ni clases: cada habilidad se aprende construyendo proyectos y
haciendo que otros estudiantes los revisen. Eso me ha dado una base sólida de
bajo nivel en C, C++, Linux, procesos, redes y Docker.

Ahora me centro en la **investigación y el desarrollo aplicado en IA**: conseguir
que modelos de lenguaje pequeños que funcionan en local trabajen juntos, que
cada petición vaya al modelo adecuado y que se verifiquen entre ellos. Mi
objetivo es trabajar en **infraestructura de IA y operaciones de centros de
datos**, donde se encuentran el bajo nivel y la IA.

---

## Proyectos principales

### Smart Routing
**Una herramienta de línea de comandos para ejecutar y enrutar modelos de lenguaje locales.**
Los modelos funcionan en local en tu máquina, sin enviar datos a servicios externos. Creas bots, das a cada uno un rol y un modelo, y la CLI envía
cada petición al que corresponde. Incluye 12 perfiles de agente (desarrollador,
depurador, investigador, redactor técnico, etc.) y 7 modos de "pensamiento
profundo" (planificación, debate, depuración de errores, razonamiento paso a
paso) que hacen una pasada de análisis antes de la respuesta final.

`Python` `LLM` `CLI` · Estado: terminando la v1.0

### Infraestructura agéntica
**Una red de agentes de IA, cada uno dentro de su propio contenedor Docker desechable.**
En lugar de un modelo grande que lo hace todo, un orquestador central divide la
petición en subtareas pequeñas. Cada subtarea se convierte en un vector
(embedding), los vectores se agrupan con k-means y cada grupo se convierte en
una rama de un árbol de agentes. Los agentes se intercambian resultados con un
contrato JSON estricto, un agente verificador revisa el trabajo de los demás, y
cada contenedor se destruye al terminar su tarea, de forma que siempre trabaja
con un contexto pequeño y limpio.

`Docker` `Embeddings` `k-means` `Multiagente` · Estado: en desarrollo

### Green Islands
**Detección de zonas verdes urbanas a partir de imágenes de satélite.**
Usa imágenes Landsat y el índice de vegetación NDVI para medir cuánta vegetación
tiene cada zona, y después agrupa las zonas con clustering no supervisado
(K-Means y DBSCAN) para encontrar "islas verdes" dentro de las ciudades. Incluye
una pequeña aplicación web para explorar y presentar los resultados.

`Python` `Jupyter` `scikit-learn` `Teledetección` · Estado: documentando el clustering

### Political NLP
**Análisis del discurso político con procesamiento del lenguaje natural.**

`Python` `NLP` · Estado: refactorizando y preparando un ejemplo claro

<sub>Estos repositorios de momento son privados y puedo enseñarlos en una entrevista.</sub>

---

## 42 Barcelona: Common Core

El Common Core es la parte obligatoria del currículum de 42. Se organiza en
**rangos del 0 al 6**. Cada rango tiene unos proyectos y, a partir del rango 2,
un examen en el que programas solo, sin internet y con tiempo limitado. Cada
proyecto lo revisan otros estudiantes y un sistema de tests automáticos (la
"Moulinette"). Terminar el Common Core es el paso previo a elegir una
especialización, como la rama de IA.

| Rango | Proyecto | Qué enseña | Repo |
|:--:|:--|:--|:--|
| 0 | **libft** | Reescribir las funciones básicas de la librería estándar de C: memoria, cadenas, listas enlazadas | [libft](https://github.com/acarranz-dev/libft) |
| 1 | **ft_printf** | Recrear `printf`: funciones variádicas y formato de salida | [ft_printf](https://github.com/acarranz-dev/ft_printf) |
| 1 | **get_next_line** | Leer un fichero línea a línea: descriptores de fichero, buffers y variables estáticas | [get_next_line](https://github.com/acarranz-dev/get_next_line) |
| 1 | **Born2beroot** | Montar un servidor Debian seguro en una máquina virtual: usuarios, cortafuegos, SSH | — |
| 2 | **push_swap** | Ordenar números con dos pilas y el mínimo de movimientos: algoritmos y complejidad | [push_swap](https://github.com/acarranz-dev/push_swap) |
| 2 | **so_long** *(o fdf / fract-ol)* | Un pequeño juego 2D: bucle gráfico, eventos y texturas | [solong](https://github.com/acarranz-dev/solong) |
| 2 | **pipex** *(o minitalk)* | Recrear las pipes de la shell con `fork`, `pipe` y `execve` | — |
| 3 | **minishell** | Una shell funcional como Bash: parsing, pipes, redirecciones, variables de entorno y señales | [minishell](https://github.com/acarranz-dev/minishell) |
| 3 | **philosophers** | El problema de los filósofos comensales: hilos, mutex y condiciones de carrera | [philosophers](https://github.com/acarranz-dev/philosophers) |
| 4 | **cub3D** *(o miniRT)* | Un motor 3D por raycasting, como Wolfenstein 3D: matemáticas, renderizado y colisiones | [cube3D](https://github.com/acarranz-dev/cube3D) |
| 4 | **NetPractice** | Configurar redes pequeñas: direcciones IP, máscaras de subred y enrutamiento | — |
| 4 | **Módulos C++ 00–04** | Programación orientada a objetos: clases, referencias, sobrecarga de operadores, herencia, polimorfismo | [cpp-modules](https://github.com/acarranz-dev/cpp-modules) |
| 5 | **Módulos C++ 05–09** | Excepciones, casts, templates, contenedores y la STL | [cpp-modules](https://github.com/acarranz-dev/cpp-modules) |
| 5 | **Inception** | Una pequeña infraestructura con Docker Compose: NGINX con TLS, WordPress y MariaDB, cada uno en su contenedor | [inception](https://github.com/acarranz-dev/inception) |
| 5 | **ft_irc** *(o webserv)* | Un servidor IRC en C++98: sockets, E/S no bloqueante con `poll` y muchos clientes a la vez | [ft_irc](https://github.com/acarranz-dev/ft_irc) |
| 6 | **ft_transcendence** | Una aplicación web completa en equipo: juego multijugador en tiempo real, autenticación y seguridad | — |

<sub>Los proyectos en *cursiva* indican las alternativas entre las que se puede
elegir. "—" significa que el proyecto no está publicado en GitHub.</sub>

---

## Qué estoy aprendiendo

| Curso | Plataforma | Para qué | Estado |
|:--|:--|:--|:--|
| **Python PCAP** (Certified Associate in Python Programming) | Python Institute / Edube | Python avanzado: módulos, POO, excepciones | En curso |
| **Hugging Face NLP Course** | Hugging Face | Fine-tuning con PEFT / LoRA y cuantización de modelos | El siguiente |
| **NLP Specialization** | DeepLearning.AI (Coursera) | Las matemáticas de los embeddings y los espacios vectoriales | Previsto |
| **Building Transformer-Based Applications** | NVIDIA Deep Learning Institute | Arquitectura Transformer | Previsto |

En 42, el siguiente paso es la **rama de Inteligencia Artificial**.

---

## Otros trabajos

- **Webs de clientes en producción**: sistemas de reservas para negocios con
  cita previa, una tienda online y la web de un escritor, hechas con Next.js.
- **Demos y experimentos**: un monitor del mercado de Steam y juegos de navegador.

---

## Tecnologías y conceptos

Solo lo que sé explicar y usar por mi cuenta.

| Área | Tecnologías y conceptos |
|:--|:--|
| **Lenguajes de programación** | **C** (todo el Common Core de 42) · **C++** (ft_irc, módulos de C++) · **Python** (Smart Routing, ciencia de datos, laboratorios de computación cuántica) · **TypeScript / JavaScript** (aplicaciones web y backends con Node.js) · **Bash** |
| **Inteligencia artificial** | **Modelos de lenguaje (LLM)**: ejecutarlos en local y por API, diseño de prompts y roles de agente · **sistemas multiagente**: repartir tareas entre agentes y verificación cruzada · **embeddings** y similitud vectorial (distancia coseno) · **clustering** con scikit-learn (K-Means, DBSCAN) · **PyTorch** · **Claude Code** y **MCP** (Model Context Protocol) |
| **Datos y ciencia** | **NumPy** · **Matplotlib** · **Jupyter** · imágenes de satélite (Landsat) y el índice de vegetación **NDVI** · computación cuántica con **Qiskit** (cúbits, puertas, estados de Bell) |
| **Web y backend** | **React** · **Next.js** · **Tailwind CSS** · **APIs REST** con **Node.js / Express** y **Flask** · **autenticación** (sesiones, contraseñas con hash, 2FA) · pagos con **Stripe** |
| **Infraestructura y DevOps** | **Docker** y **Docker Compose** · **NGINX** con TLS · **Linux** · **Git** y **GitHub** · **GitHub Actions** · **Vercel** · **AWS S3** |
| **Conceptos de sistemas** | **memoria y punteros** (stack, heap, fugas) · **procesos y señales** (`fork`, `execve`, pipes, redirecciones) · **hilos y mutex** (condiciones de carrera) · **sockets y redes** (TCP/IP, `poll`, direcciones IP y subredes) |

<p align="center">
  <img src="https://skillicons.dev/icons?i=c,cpp,py,ts,js,bash,linux,git,github,githubactions,docker,nginx&perline=12" alt="Languages, systems and infrastructure" /><br/>
  <img src="https://skillicons.dev/icons?i=pytorch,sklearn,nodejs,express,flask,nextjs,react,tailwind,aws,vercel&perline=12" alt="AI, web and cloud" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square&logo=anthropic&logoColor=white" alt="Claude Code" />
  <img src="https://img.shields.io/badge/MCP-000000?style=flat-square" alt="MCP" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white" alt="Jupyter" />
  <img src="https://img.shields.io/badge/Qiskit-6929C4?style=flat-square&logo=qiskit&logoColor=white" alt="Qiskit" />
  <img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe" />
</p>
