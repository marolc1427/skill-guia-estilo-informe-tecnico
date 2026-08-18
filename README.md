# Guía de estilo para informes técnicos

Skill que impone reglas concretas de
redacción, tipografía, figuras, tablas y estructura al escribir o revisar informes
técnicos y académicos.

## Para qué se utiliza

- Redactar secciones nuevas de un informe técnico siguiendo un estilo normativo fijo
  (introducción, metodología, figuras, tablas, ecuaciones...).
- Revisar un borrador ya existente y detectar incumplimientos concretos (con
  ubicación), por ejemplo: títulos mal capitalizados, negritas indebidas, referencias
  cruzadas fuera de orden, figuras en formato no vectorial, tablas sin estilo
  booktabs, ecuaciones numeradas sin necesidad, etc.
- Revisar el maquetado final de un documento (LaTeX) antes de la entrega.

## Cuándo se utiliza

Se activa automáticamente cuando, dentro de un proyecto con esta skill instalada, se
pide a Claude tareas como:

- "Redacta la introducción/metodología de este informe."
- "Revisa el estilo de este TFG/memoria."
- "Corrige el formato de las figuras y tablas del informe."
- "Dale un repaso al maquetado antes de entregar el documento."

No aplica a documentación técnica de software (READMEs, docstrings, comentarios de
código) ni a comunicaciones informales; está pensada específicamente para informes
técnicos/académicos formales.

## Cómo utilizarla

Esta skill se instala clonando (o copiando) este repositorio dentro de la carpeta
`.claude/skills/` del proyecto donde se va a redactar o revisar el informe. La
estructura final del proyecto debe quedar así:

```
mi-proyecto/
├── claude.md
├── .claude/
│   └── skills/
│       ├── mi-skill-personal/
│       │   └── SKILL.md
│       └── guia-estilo-informe-tecnico/     <- este repositorio
│           ├── SKILL.md
│           └── README.md
├── src/
└── [otros archivos del proyecto]
```

### Pasos

1. Sitúate en la raíz de tu proyecto (donde vive `claude.md` o donde vayas a trabajar
   con Claude Code).
2. Crea la carpeta de skills si no existe:

   ```bash
   mkdir -p .claude/skills
   ```

3. Clona este repositorio directamente dentro de `.claude/skills/` con el nombre de la
   skill:

   ```bash
   git clone <URL-de-este-repositorio> .claude/skills/guia-estilo-informe-tecnico
   ```

   Si no usas git, también vale copiar la carpeta a mano; lo único imprescindible es
   que `SKILL.md` quede en `.claude/skills/guia-estilo-informe-tecnico/SKILL.md`.

4. Abre Claude Code en ese proyecto. La skill se
   detecta automáticamente por su ubicación; no requiere configuración adicional.
5. Pide la tarea con normalidad ("revisa el estilo de mi informe en `informe.tex`",
   "redacta la metodología a partir de estas secciones..."). Claude cargará las reglas
   de `SKILL.md` y las aplicará.

### Actualizar la skill

Si el repositorio se actualiza con nuevas reglas, basta con hacer `git pull` dentro de
`.claude/skills/guia-estilo-informe-tecnico/`.