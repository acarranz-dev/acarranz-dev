<div align="center">

# Andreu Carranza

**AI R&D · Agentic systems · Systems programming at 42 Barcelona**

**English** · [Català](README.ca.md) · [Español](README.es.md)

[![42 Barcelona](https://img.shields.io/badge/42-Barcelona-000000?style=for-the-badge&logo=42&logoColor=white)](https://www.42barcelona.com)
[![Location](https://img.shields.io/badge/Catalonia-Spain-1f6feb?style=for-the-badge)](#)
[![Email](https://img.shields.io/badge/Email-contact-ea4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:andreucarranzagibert@gmail.com)

</div>

---

## About me

I am a software developer trained at **42 Barcelona**, a peer-to-peer school with
no teachers and no classes: every skill is learned by building projects and
having them reviewed by other students. That gave me a solid low-level base in
C, C++, Linux, processes, networking and Docker.

Today I focus on **applied AI research and development**: making small language
models that run locally work together, route each request to the right model,
and be verified by each other. My goal is to work in **AI infrastructure and
data center operations**, where low-level knowledge and AI meet.

---

## Main projects

### Smart Routing
**A command-line tool for running and routing local language models.**
It runs on top of [Ollama](https://ollama.com), so everything works offline on
your own machine. You create bots, give each one a role and a model, and the CLI
sends every request to the right one. It ships with 12 agent profiles
(developer, debugger, researcher, technical writer, etc.) and 7 "deep thinking"
modes (planning, debate, error debugging, step-by-step reasoning) that run an
analysis pass before the final answer.

`Python` `Ollama` `LLM` `CLI` · Status: finishing v1.0

### Agentic Infrastructure
**A network of AI agents, each living in its own short-lived Docker container.**
Instead of one big model doing everything, a central orchestrator splits the
request into small subtasks. Each subtask is turned into a vector (embedding),
the vectors are grouped with k-means, and each group becomes a branch of an
agent tree. Agents exchange results through a strict JSON contract, a dedicated
verifier agent checks the work of the others, and every container is destroyed
when its task is done, so each one always works with a small, clean context.

`Docker` `Redis` `Embeddings` `k-means` `Multi-agent` · Status: in development

### Green Islands
**Detecting urban green areas from satellite images.**
Uses Landsat imagery and the NDVI vegetation index to measure how much
vegetation each area has, then groups areas with unsupervised clustering
(K-Means and DBSCAN) to find "green islands" inside cities. Includes a small web
app to explore and present the results.

`Python` `Jupyter` `scikit-learn` `Remote sensing` · Status: documenting the clustering

### Political NLP
**Analysing political discourse with natural language processing.**

`Python` `NLP` · Status: refactoring and preparing a clear example

<sub>These repositories are private for now and can be shown in an interview.</sub>

---

## 42 Barcelona: Common Core

The Common Core is the mandatory part of the 42 curriculum. It is organised in
**ranks 0 to 6**. Each rank has a set of projects and, from rank 2 onwards, an
exam in which you code alone, without internet, against a timer. Every project
is reviewed by other students and by an automated test suite (the "Moulinette").
Finishing the Common Core is the step before choosing a specialisation, such as
the AI branch.

| Rank | Project | What it teaches | Repo |
|:--:|:--|:--|:--|
| 0 | **libft** | Rewriting the basic functions of the C standard library: memory, strings, linked lists | [libft](https://github.com/acarranz-dev/libft) |
| 1 | **ft_printf** | Recreating `printf`: variadic functions and output formatting | [ft_printf](https://github.com/acarranz-dev/ft_printf) |
| 1 | **get_next_line** | Reading a file line by line: file descriptors, buffers and static variables | [get_next_line](https://github.com/acarranz-dev/get_next_line) |
| 1 | **Born2beroot** | Setting up a secure Debian server in a virtual machine: users, firewall, SSH | — |
| 2 | **push_swap** | Sorting numbers with two stacks and as few moves as possible: algorithms and complexity | [push_swap](https://github.com/acarranz-dev/push_swap) |
| 2 | **so_long** *(or fdf / fract-ol)* | A small 2D game: graphics loop, events and textures | [solong](https://github.com/acarranz-dev/solong) |
| 2 | **pipex** *(or minitalk)* | Recreating shell pipes with `fork`, `pipe` and `execve` | — |
| 3 | **minishell** | A working shell like Bash: parsing, pipes, redirections, environment variables and signals | [minishell](https://github.com/acarranz-dev/minishell) |
| 3 | **philosophers** | The dining philosophers problem: threads, mutexes and race conditions | [philosophers](https://github.com/acarranz-dev/philosophers) |
| 4 | **cub3D** *(or miniRT)* | A 3D engine using raycasting, like Wolfenstein 3D: maths, rendering and collisions | [cube3D](https://github.com/acarranz-dev/cube3D) |
| 4 | **NetPractice** | Configuring small networks: IP addressing, subnet masks and routing | — |
| 4 | **C++ modules 00–04** | Object-oriented programming: classes, references, operator overloading, inheritance, polymorphism | [cpp-modules](https://github.com/acarranz-dev/cpp-modules) |
| 5 | **C++ modules 05–09** | Exceptions, casts, templates, containers and the STL | [cpp-modules](https://github.com/acarranz-dev/cpp-modules) |
| 5 | **Inception** | A small infrastructure with Docker Compose: NGINX with TLS, WordPress and MariaDB, each in its own container | [inception](https://github.com/acarranz-dev/inception) |
| 5 | **ft_irc** *(or webserv)* | An IRC server in C++98: sockets, non-blocking I/O with `poll` and many clients at once | [ft_irc](https://github.com/acarranz-dev/ft_irc) |
| 6 | **ft_transcendence** | A full web application in a team: real-time multiplayer game, authentication and security | — |

<sub>Projects in *italics* list the alternatives a student can choose between.
"—" means the project is not published on GitHub.</sub>

---

## Currently learning

| Course | Platform | What for | Status |
|:--|:--|:--|:--|
| **Python PCAP** (Certified Associate in Python Programming) | Python Institute / Edube | Advanced Python: modules, OOP, exceptions | In progress |
| **Hugging Face NLP Course** | Hugging Face | Fine-tuning with PEFT / LoRA and model quantization | Next |
| **NLP Specialization** | DeepLearning.AI (Coursera) | The maths behind embeddings and vector spaces | Planned |
| **Building Transformer-Based Applications** | NVIDIA Deep Learning Institute | Transformer architecture | Planned |

At 42, the next step is the **Artificial Intelligence branch**.

---

## Other work

- **Client websites in production**: booking systems for appointment-based
  businesses, an online shop and an author's website, built with Next.js.
- **Demos and experiments**: 3D body scanning from a webcam, a Steam market
  monitor, browser games and Godot prototypes.

---

## Tools

<p align="center">
  <img src="https://skillicons.dev/icons?i=c,cpp,python,ts,bash,linux,docker,git,nextjs,postgres&perline=10" alt="C, C++, Python, TypeScript, Bash, Linux, Docker, Git, Next.js, PostgreSQL" />
</p>
