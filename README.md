# 🔄 Metodología SCRUM: Guía Definitiva de Gestión Ágil

![Scrum Badge](https://img.shields.io/badge/Metodología-SCRUM-blue?style=for-the-badge&logo=agile)
![Nivel](https://img.shields.io/badge/Nivel-Principiante_a_Avanzado-success?style=for-the-badge)
![Equipo](https://img.shields.io/badge/Para-Equipos_de_Desarrollo-orange?style=for-the-badge)

Bienvenidos a la guía de referencia rápida del equipo para la gestión de proyectos usando el framework SCRUM. Aquí documentamos nuestros procesos, roles y ceremonias.

---

## 📑 Tabla de Contenidos
1. [¿Qué es SCRUM?](#1-qué-es-scrum)
2. [El Motor de SCRUM (Pilares)](#2-el-motor-de-scrum-pilares)
3. [Los Roles (El Equipo)](#3-los-roles-el-equipo)
4. [Artefactos (Herramientas de Gestión)](#4-artefactos-herramientas-de-gestión)
5. [Eventos (Ceremonias)](#5-eventos-ceremonias)
6. [Historias de Usuario y Framework INVEST](#6-historias-de-usuario-y-framework-invest)

---

## 🧠 1. ¿Qué es SCRUM?

### 🌱 Nivel Junior (La Analogía)
Imagina que nos encargan construir un coche nuevo. En lugar de encerrarnos en un garaje durante dos años y rezar para que al cliente le guste el resultado final, en SCRUM construimos primero un monopatín, a las dos semanas se lo enseñamos al cliente; luego le ponemos un manillar (patinete), luego pedales (bicicleta)... y así hasta llegar al coche. Dividimos un proyecto gigante en trozos pequeños, entregando partes que **funcionan** frecuentemente.

### 🚀 Nivel Senior (Profundidad Técnica)
SCRUM es un *framework* ágil e iterativo fundamentado en el **control empírico de procesos** y el pensamiento *Lean*. Mitiga el riesgo de desarrollo al imponer ciclos cortos de tiempo (*time-boxing*) que garantizan una entrega continua de valor (ROI temprano) y adaptabilidad total ante la variabilidad de los requisitos del mercado o del stack tecnológico.

---

## ⚙️ 2. El Motor de SCRUM (Pilares)

La lógica subyacente de SCRUM no es hacer reuniones por hacer. El framework compila gracias a tres pilares inquebrantables:

* 👁️ **Transparencia:** Todo el equipo ve el estado real del proyecto (usando tableros como Jira, GitHub Projects o Trello).
* 🔍 **Inspección:** Revisamos constantemente qué hemos construido y cómo lo hemos hecho.
* 🔀 **Adaptación:** Si algo falla o el requerimiento cambia, pivotamos inmediatamente en el siguiente ciclo.

---

## 🧑‍🤝‍🧑 3. Los Roles (El Equipo)

En SCRUM no hay "Jefes de Proyecto". La autoridad está distribuida:

| Rol | Responsabilidad Principal | Detalles |
| :--- | :--- | :--- |
| 👑 **Product Owner (PO)** | Maximizar el Valor | Es la voz del cliente. Único dueño del *Product Backlog*. Decide **QUÉ** se va a hacer y prioriza las tareas. |
| 🛡️ **Scrum Master (SM)** | Facilitar el Proceso | Es un *Servant-Leader*. Elimina bloqueos, asegura que se respeten las reglas de SCRUM y protege al equipo. |
| 💻 **Developers** | Construir el Producto | Equipo multidisciplinar (Devs, QA, DevOps, UI/UX). Se auto-organizan para decidir **CÓMO** se ejecuta el trabajo técnico. |

---

## 📦 4. Artefactos (Herramientas de Gestión)

Son los elementos que nos permiten dar transparencia al flujo de trabajo:

1. 📚 **Product Backlog:** La lista viva, ordenada y priorizada por el PO con TODO lo que el producto necesita (features, bugs, refactorizaciones).
2. 🎯 **Sprint Backlog:** El plan de batalla a corto plazo. Es el subconjunto de tareas que los Developers seleccionan y se comprometen a terminar en el Sprint actual.
3. 🎁 **Incremento:** El código en producción (o listo para ello). Es la suma de todos los elementos completados en el Sprint. **Debe ser 100% funcional**.

---

## 📅 5. Eventos (Ceremonias)

Nuestros ciclos de trabajo se dividen en los siguientes *Time-boxes*:

* 🏃 **El Sprint:** El contenedor principal. Generalmente de 2 a 4 semanas. Durante este tiempo no se pueden alterar los objetivos.
* 🗺️ **Sprint Planning:** Reunión al inicio. El PO explica el objetivo y el equipo de desarrollo define el *Sprint Backlog* (qué pueden asumir y cómo lo harán).
* ⏱️ **Daily Scrum (Daily):** Sincronización diaria de **15 minutos** exclusiva para Developers. Cada uno responde: *¿Qué hice ayer? ¿Qué haré hoy? ¿Tengo bloqueos?*
* 🔍 **Sprint Review:** Al final del Sprint. Mostramos el **Incremento** funcionando a los *Stakeholders* para recibir feedback directo.
* 🔄 **Sprint Retrospective:** Reunión interna del equipo para analizar procesos, herramientas y relaciones. Buscamos al menos 1 mejora accionable para el próximo Sprint.

---

## 📝 6. Historias de Usuario y Framework INVEST

Las tareas no se escriben con lenguaje técnico oscuro, sino como **Historias de Usuario** desde la perspectiva del cliente final.

### El Framework INVEST
Toda historia de nuestro Backlog debe cumplir esto antes de entrar a un Sprint:
* **I**ndependiente (No bloqueada por otras).
* **N**egociable (Abierta a discusión técnica).
* **V**aliosa (Aporta impacto real).
* **E**stimable (Podemos medir su complejidad en Story Points).
* **S**mall (Pequeña, cabe dentro de un solo Sprint).
* **T**esteable (Tiene criterios claros de validación).

### 📋 Template Estándar para nuestros Issues / Tickets

> 💡 *Usa este formato al crear nuevos tickets en nuestro tablero de GitHub/Jira.*

```markdown
### 🏷️ Historia de Usuario: [Título Corto]

**Como** [Tipo de Usuario]
**Quiero** [Acción / Funcionalidad]
**Para** [Beneficio / Valor de negocio]

---

#### ✅ Criterios de Aceptación (Acceptance Criteria)
*Reglas específicas de negocio que el QA/PO validará:*
1. [Ej: Si el email es inválido, mostrar alerta roja.]
2. [Ej: El enlace debe expirar en 15 minutos.]

---

#### 🏁 Definition of Done (DoD)
*Estándar global del equipo:*
- [ ] El código pasa el linter y no tiene *code smells*.
- [ ] Pruebas unitarias implementadas.
- [ ] PR aprobado por al menos 1 compañero.
- [ ] Desplegado en el entorno de `Staging`.
