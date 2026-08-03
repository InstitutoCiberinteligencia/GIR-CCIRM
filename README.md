<p align="center">
  <img src="assets/Oneiros-light-horizontal.png" alt="Oneiros Academy" width="420">
</p>

<h1 align="center">GIR + CCIRM Lab</h1>

<p align="center">
  <em>Un laboratorio interactivo de 115 minutos para convertir amenazas priorizadas en una agenda de inteligencia y un plan de obtención: GIR → PIR/EEI → CMF → ICP/IAP.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Duraci%C3%B3n-115%20min-7FD4B4">
  <img src="https://img.shields.io/badge/Formato-HTML%20%C3%BAnico-92CDE6">
  <img src="https://img.shields.io/badge/Sin%20dependencias-offline-5FBF9E">
  <img src="https://img.shields.io/badge/Licencia-CC%20BY--NC%204.0-6FC9C2">
  <img src="https://img.shields.io/badge/Oneiros-Academy-6FC9C2">
</p>

---

## ¿Qué es esto?

Un taller práctico de **Dirección de Inteligencia** para trabajar en grupo sobre un caso realista (la institución financiera ficticia *FinBank Digital*). Los participantes recorren la cadena completa que va desde una amenaza priorizada hasta un plan de obtención ejecutable: qué necesita saber la organización, en qué orden, con qué fuentes, quién lo busca y qué capacidad falta habilitar.

Es la **continuación natural del [Threat Modeling Lab](https://github.com/InstitutoCiberinteligencia/Threat-Modeling)**: aquel produce escenarios de amenaza priorizados; este los convierte en requerimientos de inteligencia. Puede usarse igualmente de forma independiente, con la ruta de ataque de referencia incluida en el propio taller. La taxonomía que alimenta la fase 4 está documentada en [CU-GIRH Reference](https://github.com/InstitutoCiberinteligencia/CU-GIRH-Reference).

Todo está contenido en **un único archivo HTML** que funciona sin conexión, sin instalaciones y sin dependencias: solo se abre en el navegador.

## La cadena, de punta a punta

Cada etapa consume la salida de la anterior. El taller no explica los conceptos por separado: obliga a encadenarlos.

| Etapa | Pregunta que responde | Aporte en el taller |
|-------|----------------------|---------------------|
| **GIR** | ¿Qué observar siempre? | Requerimiento general y permanente, seleccionado del catálogo CU-GIRH. |
| **PIR / EEI** | ¿Qué pregunta, ahora? | Necesidad priorizada, formulada como pregunta y descompuesta en elementos esenciales. |
| **CMF** | ¿Puedo responderlo? | Diagnóstico de cobertura: fuentes disponibles y brechas de visibilidad. |
| **ICP** | ¿Quién busca y cuándo? | Plan de obtención sobre las capacidades que ya existen. |
| **IAP** | ¿Qué me falta ver? | Plan de adquisición para habilitar la fuente, el sensor o el acceso que falta. |

El bloque **PIR/EEI → CMF → ICP/IAP** es lo que la doctrina denomina **CCIRM** (*Collection Coordination and Intelligence Requirements Management*). El GIR es la entrada; el CCIRM es el trabajo.

## Características

- **Catálogo CU-GIRH completo** integrado como autocompletado: más de 500 GIRs con validación en vivo (si el texto no coincide con un GIR real, el campo se marca y no puntúa).
- **Motor de priorización transparente**: el puntaje de cada PIR se calcula con `Peso + 110 − (Rango × 10)`, y la consolidación bonifica los GIRs que varios stakeholders piden. Las fórmulas están a la vista, no ocultas.
- **Collection Guidance en vivo**: cambia el peso de un stakeholder y el top-20 del equipo se reordena al instante.
- **Router de obtención**: la columna *Visibilidad* del CMF (Sí / Parcial / No) enruta automáticamente cada requerimiento al **ICP** o al **IAP**. La bifurcación no se explica en una lámina: se ejecuta.
- **Navegación por fases** con botones *Siguiente / Atrás*, barra de progreso y atajos de teclado (`←` / `→`).
- **Cronómetro por fase** que carga automáticamente el tiempo sugerido; el facilitador lo inicia, pausa o reinicia.
- **Cierre en formato BLUF** con NLT, LTIOV, duración del ciclo y cadencia de SITREP.
- **Exportación a PDF** con guía paso a paso integrada, que muestra el contenido completo de cada campo.
- **Identidad visual de Oneiros Academy** y diseño responsive.

## Cómo usarlo

> ℹ️ **Importante:** la vista normal del archivo en GitHub muestra el *código fuente*, no el taller. Para abrir el laboratorio usa una de estas opciones.

### Opción A — Descargar y abrir (recomendada para alumnos)

1. Abre el archivo y haz clic en **Download raw file**, o descarga directamente desde:
   `https://github.com/InstitutoCiberinteligencia/GIR-CCIRM/raw/refs/heads/main/GIR_CCIRM_Lab.html`
2. Haz doble clic en el archivo descargado: se abre en tu navegador.
3. ¡Listo! No requiere internet ni instalación.

### Opción B — Abrir directo en el navegador (GitHub Pages)

Disponible on-line en:

```
https://institutociberinteligencia.github.io/GIR-CCIRM/GIR_CCIRM_Lab.html
```

## Flujo del taller (10 fases · ~115 min)

| # | Fase | Tiempo | Etapa | Resultado |
|---|------|:------:|-------|-----------|
| 1 | Inicio | 8 min | Contexto | Objetivos y cadena de Dirección |
| 2 | El caso | 8 min | Contexto | FinBank Digital y ruta de ataque |
| 3 | Stakeholders | 10 min | Dirección | Lista de unidades con peso asignado |
| 4 | GIRs → PIRs | 20 min | GIR | Hasta 8 GIRs rankeados por stakeholder |
| 5 | Collection Guidance | 10 min | GIR | Top-20 consolidado y deduplicado |
| 6 | PIR → EEI | 15 min | PIR/EEI | 3 GIRs convertidos en pregunta y desglosados |
| 7 | Matriz de cobertura | 12 min | CMF | Fuentes, alcance, cadencia y brechas |
| 8 | ICP | 12 min | Obtención | Tareas con responsable, prioridad y plazo |
| 9 | IAP | 10 min | Obtención | Capacidades a habilitar para cerrar brechas |
| 10 | Cierre | 10 min | Difusión | Síntesis BLUF y ritmo de batalla |

## Guía rápida para el facilitador

- Proyecta el archivo y avanza en conjunto fase por fase.
- Forma grupos de **4 a 6 personas**; cada integrante representa a un stakeholder (Dirección, SOC, Incident Response, Fraude, Vulnerability Management, Riesgo). El peso de cada uno altera la prioridad resultante.
- Usa el **cronómetro** para mantener el ritmo; cada grupo trabaja sus propias hojas.
- La fase 4 es la más larga y la que más se dispersa: recuerda que rankear mal es peor que rankear poco. *Si todo es prioridad, nada es prioridad.*
- La discusión más rica aparece en la fase 7: los grupos tienden a marcar «Sí» por optimismo. Pregunta por retención de logs, cobertura de endpoints Linux y acceso a fuentes underground antes de dejarlos avanzar.
- En el cierre, cada grupo presenta su BLUF en **2 minutos**. Si necesita más de dos líneas para explicar la conclusión, no es un BLUF.

> ⚠️ **Importante:** el contenido que se escribe vive solo durante la sesión del navegador (no se guarda al recargar). Si un grupo necesita conservar su trabajo, debe **exportar a PDF** antes de cerrar la pestaña.

## Exportación a PDF

El taller incluye una guía paso a paso en la fase de cierre. Los dos ajustes que deciden si el entregable se ve completo:

- **Escala: personalizada 70 %** — no uses *«Ajustar al ancho de página»*, recorta las tablas del CMF y del ICP por el lado derecho.
- **Gráficos de fondo: activados** — sin esto se pierden los colores de prioridad y los chips de visibilidad.

## Estructura del repositorio

```
.
├── GIR_CCIRM_Lab.html                 # El laboratorio (todo en un archivo)
├── assets/
│   └── Oneiros-light-horizontal.png   # Logo para este README
├── LICENSE                            # CC BY-NC 4.0
└── README.md
```

## Repositorios relacionados

Este laboratorio es la segunda pieza de una secuencia de tres que se usan en orden:

| Repositorio | Rol en la secuencia |
|-------------|---------------------|
| [Threat Modeling Lab](https://github.com/InstitutoCiberinteligencia/Threat-Modeling) | **Antes.** Identifica el riesgo: produce los escenarios de amenaza priorizados que este taller consume como insumo. |
| **GIR + CCIRM Lab** *(este repo)* | Convierte esos escenarios en requerimientos priorizados y en un plan de obtención. |
| [CU-GIRH Reference](https://github.com/InstitutoCiberinteligencia/CU-GIRH-Reference) | **Durante.** Índice navegable de la taxonomía CU-GIRH y guía para convertir GIRs en PIRs y EEIs. |

Los tres son autónomos: puedes ejecutar este taller sin haber hecho el anterior, usando la ruta de ataque de referencia incluida en la fase 2.

## Créditos

Desarrollado para **Oneiros Academy** como material de formación en ciberseguridad e inteligencia de amenazas.

La taxonomía de requerimientos utilizada es el **CU-GIRH** (*Cyber Underground General Intelligence Requirements Handbook*) v7.0, publicado por **Intel 471, Inc.** bajo licencia CC BY-NC-ND 4.0 y empleado aquí con fines exclusivamente formativos. El handbook completo se descarga en <https://www.intel471.com/cyber-underground-handbook>; el índice navegable de códigos está en [CU-GIRH Reference](https://github.com/InstitutoCiberinteligencia/CU-GIRH-Reference).

Este repositorio no está afiliado a Intel 471, Inc., ni patrocinado ni respaldado por dicha empresa.

## Licencia

Este material se distribuye bajo licencia **Creative Commons Atribución-NoComercial 4.0 Internacional (CC BY-NC 4.0)**: puedes compartirlo y adaptarlo dando crédito, pero no usarlo con fines comerciales. Consulta el archivo [`LICENSE`](LICENSE) para más detalles.

---

<p align="center"><sub>Oneiros Academy · GIR + CCIRM Lab</sub></p>
