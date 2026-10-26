<div align="center">

# Andreu Carranza

**Programador en C, C++ i Python format a 42 Barcelona. Dissenyo arquitectures multiagent sobre LLM: descomposició de tasques, enrutament semàntic i verificació creuada entre agents.**

[English](README.md) · **Català** · [Español](README.es.md)

[![42 Barcelona](https://img.shields.io/badge/42-Barcelona-000000?style=for-the-badge&logo=42&logoColor=white)](https://www.42barcelona.com)
[![Ubicació](https://img.shields.io/badge/Catalunya-Espanya-1f6feb?style=for-the-badge)](#)
[![Correu](https://img.shields.io/badge/Correu-contacte-ea4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:andreucarranzagibert@gmail.com)

</div>

---

## Sobre mi

Soc desenvolupador format a **42 Barcelona**, una escola entre iguals sense
professors ni classes: cada habilitat s'aprèn construint projectes i fent que
altres estudiants els revisin. Això m'ha donat una base sòlida de baix nivell en
C, C++, Linux, processos, xarxes i Docker.

Ara em centro en la **recerca i el desenvolupament aplicat en IA**: fer que models
de llenguatge petits que funcionen en local treballin junts, que cada petició
vagi al model adequat i que es verifiquin entre ells. El meu objectiu és
treballar en **infraestructura d'IA i operacions de centres de dades**, on es
troben el baix nivell i la IA.

---

## Projectes principals

### Smart Routing
**Una eina de línia d'ordres per executar i enrutar models de llenguatge locals.**
Els models funcionen en local a la teva màquina, sense enviar dades a serveis externs. Crees bots, dones a cadascun un rol i un model, i la CLI
envia cada petició al que toca. Inclou 12 perfils d'agent (desenvolupador,
depurador, investigador, redactor tècnic, etc.) i 7 modes de "pensament profund"
(planificació, debat, depuració d'errors, raonament pas a pas) que fan una
passada d'anàlisi abans de la resposta final.

`Python` `LLM` `CLI` · Estat: acabant la v1.0

### Infraestructura agèntica
**Una xarxa d'agents d'IA, cadascun dins del seu propi contenidor Docker d'un sol ús.**
En lloc d'un model gran que ho fa tot, un orquestrador central divideix la
petició en subtasques petites. Cada subtasca es converteix en un vector
(embedding), els vectors s'agrupen amb k-means i cada grup es converteix en una
branca d'un arbre d'agents. Els agents s'intercanvien resultats amb un contracte
JSON estricte, un agent verificador revisa la feina dels altres, i cada
contenidor es destrueix quan acaba la seva tasca, de manera que sempre treballa
amb un context petit i net.

`Docker` `Embeddings` `k-means` `Multiagent` · Estat: en desenvolupament

### Green Islands
**Detecció de zones verdes urbanes a partir d'imatges de satèl·lit.**
Fa servir imatges Landsat i l'índex de vegetació NDVI per mesurar quanta
vegetació té cada zona, i després agrupa les zones amb clustering no supervisat
(K-Means i DBSCAN) per trobar "illes verdes" dins de les ciutats. Inclou una
petita aplicació web per explorar i presentar els resultats.

`Python` `Jupyter` `scikit-learn` `Teledetecció` · Estat: documentant el clustering

### Political NLP
**Anàlisi del discurs polític amb processament del llenguatge natural.**

`Python` `NLP` · Estat: refactoritzant i preparant un exemple clar

<sub>Aquests repositoris de moment són privats i els puc ensenyar en una entrevista.</sub>

---

## 42 Barcelona: Common Core

El Common Core és la part obligatòria del currículum de 42. S'organitza en
**rangs del 0 al 6**. Cada rang té uns projectes i, a partir del rang 2, un
examen en què programes sol, sense internet i amb temps limitat. Cada projecte
el revisen altres estudiants i un sistema de tests automàtics (la "Moulinette").
Acabar el Common Core és el pas previ a triar una especialització, com la
branca d'IA.

| Rang | Projecte | Què ensenya | Repo |
|:--:|:--|:--|:--|
| 0 | **libft** | Reescriure les funcions bàsiques de la llibreria estàndard de C: memòria, cadenes, llistes enllaçades | [libft](https://github.com/acarranz-dev/libft) |
| 1 | **ft_printf** | Recrear `printf`: funcions variàdiques i format de sortida | [ft_printf](https://github.com/acarranz-dev/ft_printf) |
| 1 | **get_next_line** | Llegir un fitxer línia a línia: descriptors de fitxer, buffers i variables estàtiques | [get_next_line](https://github.com/acarranz-dev/get_next_line) |
| 1 | **Born2beroot** | Muntar un servidor Debian segur en una màquina virtual: usuaris, tallafocs, SSH | — |
| 2 | **push_swap** | Ordenar números amb dues piles i el mínim de moviments: algorismes i complexitat | [push_swap](https://github.com/acarranz-dev/push_swap) |
| 2 | **so_long** *(o fdf / fract-ol)* | Un petit joc 2D: bucle gràfic, esdeveniments i textures | [solong](https://github.com/acarranz-dev/solong) |
| 2 | **pipex** *(o minitalk)* | Recrear les pipes de la shell amb `fork`, `pipe` i `execve` | — |
| 3 | **minishell** | Una shell funcional com Bash: parsing, pipes, redireccions, variables d'entorn i senyals | [minishell](https://github.com/acarranz-dev/minishell) |
| 3 | **philosophers** | El problema dels filòsofs a taula: fils, mutex i condicions de carrera | [philosophers](https://github.com/acarranz-dev/philosophers) |
| 4 | **cub3D** *(o miniRT)* | Un motor 3D per raycasting, com Wolfenstein 3D: matemàtiques, renderitzat i col·lisions | [cube3D](https://github.com/acarranz-dev/cube3D) |
| 4 | **NetPractice** | Configurar xarxes petites: adreces IP, màscares de subxarxa i enrutament | — |
| 4 | **Mòduls C++ 00–04** | Programació orientada a objectes: classes, referències, sobrecàrrega d'operadors, herència, polimorfisme | [cpp-modules](https://github.com/acarranz-dev/cpp-modules) |
| 5 | **Mòduls C++ 05–09** | Excepcions, casts, templates, contenidors i la STL | [cpp-modules](https://github.com/acarranz-dev/cpp-modules) |
| 5 | **Inception** | Una petita infraestructura amb Docker Compose: NGINX amb TLS, WordPress i MariaDB, cadascun al seu contenidor | [inception](https://github.com/acarranz-dev/inception) |
| 5 | **ft_irc** *(o webserv)* | Un servidor IRC en C++98: sockets, E/S no bloquejant amb `poll` i molts clients alhora | [ft_irc](https://github.com/acarranz-dev/ft_irc) |
| 6 | **ft_transcendence** | Una aplicació web completa en equip: joc multijugador en temps real, autenticació i seguretat | — |

<sub>Els projectes en *cursiva* indiquen les alternatives entre les quals es pot
triar. "—" vol dir que el projecte no està publicat a GitHub.</sub>

---

## Què estic aprenent

| Curs | Plataforma | Per a què | Estat |
|:--|:--|:--|:--|
| **Python PCAP** (Certified Associate in Python Programming) | Python Institute / Edube | Python avançat: mòduls, POO, excepcions | En curs |
| **Hugging Face NLP Course** | Hugging Face | Fine-tuning amb PEFT / LoRA i quantització de models | El següent |
| **NLP Specialization** | DeepLearning.AI (Coursera) | Les matemàtiques dels embeddings i els espais vectorials | Previst |
| **Building Transformer-Based Applications** | NVIDIA Deep Learning Institute | Arquitectura Transformer | Previst |

A 42, el següent pas és la **branca d'Intel·ligència Artificial**.

---

## Altres treballs

- **Webs de clients en producció**: sistemes de reserves per a negocis amb cita
  prèvia, una botiga en línia i la web d'un escriptor, fetes amb Next.js.
- **Demos i experiments**: un monitor del mercat de Steam i jocs de navegador.

---

## Tecnologies i conceptes

Només el que sé explicar i fer servir pel meu compte.

| Àrea | Tecnologies i conceptes |
|:--|:--|
| **Llenguatges de programació** | **C** (tot el Common Core de 42) · **C++** (ft_irc, mòduls de C++) · **Python** (Smart Routing, ciència de dades, laboratoris de computació quàntica) · **TypeScript / JavaScript** (aplicacions web i backends amb Node.js) · **Bash** |
| **Intel·ligència artificial** | **Models de llenguatge (LLM)**: executar-los en local i per API, disseny de prompts i rols d'agent · **sistemes multiagent**: repartir tasques entre agents i verificació creuada · **embeddings** i similitud vectorial (distància cosinus) · **clustering** amb scikit-learn (K-Means, DBSCAN) · **PyTorch** · **Claude Code** i **MCP** (Model Context Protocol) |
| **Dades i ciència** | **NumPy** · **Matplotlib** · **Jupyter** · imatges de satèl·lit (Landsat) i l'índex de vegetació **NDVI** · computació quàntica amb **Qiskit** (qubits, portes, estats de Bell) |
| **Web i backend** | **React** · **Next.js** · **Tailwind CSS** · **APIs REST** amb **Node.js / Express** i **Flask** · **autenticació** (sessions, contrasenyes amb hash, 2FA) · pagaments amb **Stripe** |
| **Infraestructura i DevOps** | **Docker** i **Docker Compose** · **NGINX** amb TLS · **Linux** · **Git** i **GitHub** · **GitHub Actions** · **Vercel** · **AWS S3** |
| **Conceptes de sistemes** | **memòria i punters** (stack, heap, fuites) · **processos i senyals** (`fork`, `execve`, pipes, redireccions) · **fils i mutex** (condicions de carrera) · **sockets i xarxes** (TCP/IP, `poll`, adreces IP i subxarxes) |

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
