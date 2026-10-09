# Investigación e Implementación de Skills en Gemini
### Corporación Universitaria Unilasallista · Actividad de Seguimiento Académico

[![Institución](https://img.shields.io/badge/Unilasallista-Corporación%20Universitaria-047857)](https://www.unilasallista.edu.co/)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![Gemini](https://img.shields.io/badge/Google%20Gemini-Skills-0284c7?logo=google&logoColor=white)
![License](https://img.shields.io/badge/Uso-Académico-f59e0b)

---

## 1. Descripción General

Este repositorio reúne los productos de la **actividad de seguimiento** del programa académico de la **Corporación Universitaria Unilasallista**, cuyo propósito es **investigar, diseñar e implementar una Skill personalizada para el ecosistema de Inteligencia Artificial de Google Gemini**.

La actividad busca demostrar cómo la **modularidad de los modelos de lenguaje** permite extender sus capacidades analíticas mediante instrucciones estructuradas (skills), aplicándolas a un caso de uso profesional real. El trabajo integra:

- La **fundamentación conceptual** de las Skills y los flujos agénticos.
- El **desarrollo técnico** de una Landing Page institucional como vitrina del proyecto.
- La **implementación y validación** de la Skill mediante pruebas reproducibles.

> *"Las Skills representan la convergencia entre la intención humana y la ejecución autónoma de modelos generativos de última generación."*

---

## 2. Estructura del Repositorio

```text
landing-skill-unilasallista/
│
├── index.html                  # Landing Page principal (HTML5 + CSS3 embebido)
│
├── assets/                     # Recursos estáticos de la landing
│   ├── css/
│   │   └── styles.css          # Hoja de estilos (si se externaliza del HTML)
│   ├── img/
│   │   └── infografia-skills.png
│   └── fonts/                  # Fuentes tipográficas locales (opcional)
│
├── data/                       # Cuaderno de datos y material de análisis
│   └── cuaderno_de_datos.ipynb # Jupyter / Google Colab Notebook documentado
│
├── skills/                     # Código fuente de la Skill implementada
│   ├── SKILL.md                # Definición, instrucciones y directrices
│   └── gemini-skill.json       # Especificación / configuración de la Skill
│
├── .agents/                    # Skills instaladas para agentes de IA
│   └── skills/
│       └── documentation-and-adrs/
│           └── SKILL.md
│
├── skills-lock.json            # Registro de skills instaladas y sus versiones
└── README.md                   # Documentación técnica del proyecto (este archivo)
```

| Ruta | Descripción |
|------|-------------|
| `index.html` | Landing Page institucional con el resumen, entregables y enlaces del proyecto. |
| `assets/` | Recursos estáticos: estilos, imágenes e infografía conceptual. |
| `data/` | Cuaderno de datos (`.ipynb`) con scripts, dataset de validación y métricas. |
| `skills/` | Código fuente de la Skill para Gemini (instrucciones + configuración). |
| `.agents/` | Skills de agente instaladas en el entorno de desarrollo. |

---

## 3. Documentación del Desarrollo

### 3.1 Metodología
El desarrollo se llevó a cabo combinando **asistencia de IA agéntica** con **programación manual**, bajo el siguiente flujo de trabajo:

1. **Antigravity** se utilizó como entorno de generación asistida para estructurar el esqueleto de la interfaz y las secciones de contenido.
2. **Opencode** actuó como asistente de desarrollo en terminal, encargado de refinar el marcado, validar la estructura y aplicar buenas prácticas.
3. La **capa de estilos** y los ajustes finales de diseño se consolidaron manualmente para garantizar consistencia visual.

### 3.2 Tecnologías Utilizadas

| Tecnología | Uso |
|------------|-----|
| **HTML5** | Estructura semántica: `header`, `section`, `article`, `footer`. |
| **CSS3 moderno** | Variables CSS (`:root`), **Grid** y **Flexbox**, `clamp`, transiciones y animaciones nativas. |
| **Google Fonts** | Tipografías *Plus Jakarta Sans* y *Space Grotesk*. |
| **Font Awesome 6** | Sistema de iconografía vectorial. |

### 3.3 Decisiones de Diseño
- **Paleta "Emerald Corporate Tech":** tonos esmeralda institucionales combinados con acentos dorado y azul, transmitiendo rigor académico y modernidad tecnológica.
- **Diseño responsivo Mobile-First:** *media queries* en `992px` y `768px` que reorganizan el Grid y adaptan la navegación.
- **Accesibilidad y rendimiento:** atributos `lang`, meta `description` para SEO, `loading` diferido de recursos y navegación con `scroll-behavior: smooth`.
- **Componentización por secciones:** Hero, Acerca del Proyecto, Entregables, CTA de Repositorio y Footer institucional.

---

## 4. Implementación de la Skill

La Skill se diseñó para **adaptar el comportamiento de Gemini a un contexto profesional**, mediante un conjunto de instrucciones, directrices y reglas de sistema que orientan las respuestas del modelo.

### 4.1 Estructura de las Instrucciones

```yaml
name: gemini-professional-skill
description: Adapta Gemini al ámbito profesional/académico con razonamiento estructurado.
instructions:
  role: "Actúa como un experto en el dominio definido por la tarea."
  reasoning: "Descompón cada problema en pasos verificables antes de responder."
  format: "Entrega respuestas con encabezados, listas y ejemplos aplicados."
  constraints: "Evita ambigüedades; cita supuestos y limitaciones explícitamente."
  validation: "Verifica la consistencia de la salida antes de finalizarla."
```

### 4.2 Directrices Aplicadas
- **Definición explícita del rol:** acota la identidad y el tono esperado del modelo.
- **Razonamiento estructurado:** obliga a descomponer tareas complejas en pasos auditables.
- **Formato de salida consistente:** estandariza la presentación de resultados.
- **Restricciones y salvaguardas:** reduce alucinaciones y respuestas fuera de alcance.
- **Validadores de respuesta:** checklist de verificación previa a la entrega final.

### 4.3 Validación
La Skill fue probada en el **cuaderno de datos** (`data/cuaderno_de_datos.ipynb`) con un dataset de casos representativos, midiendo consistencia, precisión del formato y utilidad del razonamiento generado.

---

## 5. Enlaces de Interés

| Recurso | Enlace |
|---------|--------|
| 🌐 **Landing Page en vivo** | _[Pegar aquí el enlace de despliegue]_ |
| 🎬 **Video en Flow** | _[Pegar aquí el enlace del video en Flow]_ |
| 💻 **Repositorio GitHub** | _[Pegar aquí el enlace del repositorio]_ |

---

## Autoría y Reconocimientos

**Corporación Universitaria Unilasallista**
Actividad de Investigación en Inteligencia Artificial · 2026

> Proyecto de carácter académico. Todo el material aquí contenido se distribuye con fines educativos e investigativos.

---

<p align="center">
  <strong>Corporación Universitaria Unilasallista</strong><br>
  Excelencia académica · Investigación formativa · Innovación tecnológica
</p>
