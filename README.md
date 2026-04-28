<p align="center"><img src="./img/opencode.png" width="600"   alt=" " /></p>

<h4 align="right">Apr 26</h4>

<p>
  <img src="https://img.shields.io/badge/OS-Linux%20GNU-yellowgreen">
  <img src="https://img.shields.io/badge/OS-Windows%2011-blue">

</p>
<h1 align="center"> OpenCode </h1> 
<br>
OpenCode es una herramienta tipo CLI/TUI (Command Line Interface /Text User Interface) para usar modelos de IA desde la terminal, enfocada en desarrollo. Permite;

* Trabajar con IA sin navegador, directo en terminal
* Manejar sesiones, agentes y contexto de código
* Automatizar tareas (generar código, refactorizar, analizar repositorios)
* Definir agentes personalizados con reglas propias

nota: No es un modelo de IA.
Es un orquestador/interfaz para usar varios modelos de forma más controlada y productiva, especialmente en workflows técnicos

***OpenCode*** está diseñado específicamente para la programación y el desarrollo de software. Es un agente de codificación. Se enfoca en ayudarte a entender, escribir, depurar y ejecutar código dentro de repositorios reales.Se usa principalmente a través de la terminal (CLI/TUI), aplicaciones de escritorio o extensiones de IDE como VS Code.Funciona bajo un esquema de "chat + herramientas", donde tú diriges la tarea y él propone ediciones. Se integra profundamente con herramientas de desarrollo como el LSP (Language Server Protocol) para refactorizar código y GitHub Actions.

OpenCode es similiar a ```Claude Code (Anthropic)``` pero de codigo abierto, mientras que Claude Code es cerrado y es la herramienta oficial optimizada específicamente para los modelos de la familia Claude (como Sonnet 3.5 o 4).

<br>


# Table of contents
- [Table of contents](#table-of-contents)
- [Install](#install)
- [Run](#run)
- [OpenCode - Comandos](#opencode---comandos)
  - [Tabla de Comandos](#tabla-de-comandos)
  - [Gestión de agentes](#gestión-de-agentes)
  - [Sesiones](#sesiones)
  - [Conexión / autenticación](#conexión--autenticación)
  - [Import / Export](#import--export)
  - [Servidor / remoto](#servidor--remoto)
  - [Estadísticas](#estadísticas)
  - [Comandos TUI (slash)](#comandos-tui-slash)
  - [Comandos personalizados](#comandos-personalizados)
- [Troubleshooting](#troubleshooting)

<br>

# Install
Desde pagina oficial: https://opencode.ai/
```bash
npm i -g opencode-ai
```

# Run
Desde terminal
```bash
opencode
```
<br>

# OpenCode - Comandos

> :memo: **Note:** Cambiar agente entre Build / Plan (con tecla Tabulacion [TAB]) 
- Build - Agente primario por defecto con todas las herramientas habilitadas
- Plan - Agente para planificación y análisis sin hacer cambios

> :bulb: **Tip:** Usar ```@``` para realizar una búsqueda aproximada de archivos dentro del proyecto. ejemplo: ¿Cómo se maneja la autenticación en ***@packages/functions/src/api/index.ts***

> :bulb: **Tip:** Arrastre y suelte imágenes en la terminal para agregarlas al mensaje.

<br>

## Tabla de Comandos

| Comando | Tipo | Descripción |
|--------|------|------------|
| opencode | CLI | Inicia la interfaz TUI interactiva |
| opencode run "<prompt>" | CLI | Ejecuta una tarea y sale |
| opencode --continue | CLI | Continúa la última sesión |
| opencode --session <id> | CLI | Continúa una sesión específica |
| opencode --fork | CLI | Duplica sesión al continuar |
| opencode --model <provider/model> | CLI | Selecciona modelo |
| opencode --agent <name> | CLI | Usa un agente específico |

---

## Gestión de agentes

| Comando | Tipo | Descripción |
|--------|------|------------|
| opencode agent | CLI | Gestión de agentes |
| opencode agent create | CLI | Crear agente personalizado |
| opencode agent list | CLI | Listar agentes disponibles |

---

## Sesiones

| Comando | Tipo | Descripción |
|--------|------|------------|
| opencode session | CLI | Gestión de sesiones |
| opencode session list | CLI | Listar sesiones |
| /sessions | TUI | Ver sesiones desde la interfaz |

---

## Conexión / autenticación

| Comando | Tipo | Descripción |
|--------|------|------------|
| opencode auth | CLI | Gestión de credenciales |
| opencode auth login | CLI | Agregar API keys |
| /connect | TUI | Añadir proveedor/API keys (equivalente práctico) |

---

## Import / Export

| Comando | Tipo | Descripción |
|--------|------|------------|
| opencode export [id] | CLI | Exportar sesión a JSON |
| opencode import <file/url> | CLI | Importar sesión |
| /export | TUI | Exportar conversación |

---

## Servidor / remoto

| Comando | Tipo | Descripción |
|--------|------|------------|
| opencode serve | CLI | Servidor API sin interfaz |
| opencode web | CLI | Interfaz web |
| opencode attach <url> | CLI | Conectar a backend remoto |

---

## Estadísticas

| Comando | Tipo | Descripción |
|--------|------|------------|
| opencode stats | CLI | Ver uso de tokens y costos |

---

## Comandos TUI (slash)

| Comando | Tipo | Descripción |
|--------|------|------------|
| /init | TUI | Genera `AGENTS.md` |
| /help | TUI | Ayuda |
| /undo | TUI | Deshacer |
| /redo | TUI | Rehacer |
| /share | TUI | Compartir sesión |
| /exit | TUI | Salir |
| /<custom> | TUI | Ejecuta comandos personalizados definidos por el usuario |

---

## Comandos personalizados

| Comando | Tipo | Descripción |
|--------|------|------------|
| /my-command | TUI | Ejecuta un comando definido en `.opencode/command/*.md` |

<br>

More information: https://opencode.ai/docs/es

<br>

<p align="center"><img src="./img/under_construction.png" width="200"   alt=" " /></p>

<br>

# Troubleshooting
> :warning: **Warning:**

<br>

---

<div>
  <p>
    <img  align="top" width="42" style="padding:0px 0px 0px 0px;" src="./img/carjavi.png"/> Copyright &nbsp;&copy; 2023 Instinto Digital <a href="https://carjavi.github.io/" title="carjavi.github">carjavi</a>
  </p>
</div>

<p align="center">
    <a href="https://instintodigital.net/" target="_blank"><img src="./img/developer.png" height="100" alt="www.instintodigital.net"></a>
</p>


