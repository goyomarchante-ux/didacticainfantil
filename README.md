# 🎓 Portal de Recursos · Didáctica de la Educación Infantil

[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-brightgreen?logo=github)](https://pages.github.com/)
[![FP Grado Superior](https://img.shields.io/badge/M%C3%B3dulo-Did%C3%A1ctica%20de%20la%20Educaci%C3%B3n%20Infantil-rose)](https://www.todofp.es/)
[![LOMLOE](https://img.shields.io/badge/Normativa-LOMLOE%20%7C%20RD%2095%2F2022-blue)](#)
[![Arquitectura](https://img.shields.io/badge/Arquitectura-Serverless%20%2F%20Zero--Build-indigo)](#)

Aplicación Web de Página Única (**SPA - Single Page Application**) interactiva, modular y responsive diseñada para dar soporte docente y servir como centro de recursos digital para el alumnado del **Ciclo Formativo de Grado Superior en Educación Infantil (TSEI)** en el módulo profesional de **Didáctica de la Educación Infantil**.

---

## 📌 Novedades y Características Principales

- 📚 **10 Unidades Formativas (U.0 a U.9):** Desde la evaluación inicial y el periodo de adaptación, hasta el marco curricular LOMLOE, bases psicopedagógicas, DUA, rincones/ambientes, evaluación y animación socioeducativa.
- ⭐ **Sistema de "Mis Favoritos" (Almacenamiento Local):** Alumnado y profesorado pueden marcar con una estrella cualquier recurso para guardarlo en su colección personal y filtrarlo instantáneamente.
- 📽️ **Modo Pizarra Digital Interactiva (PDI) / Proyector:** Botón dedicado para el aula que amplía la tipografía, maximiza el contraste y oculta elementos secundarios para una proyección óptima.
- 🏷️ **Etiquetado Didáctico y Búsqueda Inteligente:** Recursos categorizados con etiquetas pedagógicas (`#DUA`, `#LOMLOE`, `#0a3años`, `#Montessori`, `#Tonucci`, `#Inclusión`, etc.).
- 🔄 **Sincronización en Directo con Google Sheets:** Permite al profesorado actualizar enlaces o añadir nuevos materiales directamente desde una hoja de cálculo en Google Drive sin tocar una sola línea de código.
- 📋 **Exportación rápida de datos:** Permite copiar la estructura en formato tabulado (TSV) o descargar un archivo CSV compatible con Excel y Google Sheets.
- 🔒 **Modo Docente:** Interfaz protegida para gestionar la vinculación con Google Sheets y visualizar guías didácticas de mantenimiento.
- 📱 **Diseño 100% Adaptable (Responsive):** Optimizado para smartphones, tablets, portátiles y pizarras interactivas de aula.
- ⚡ **Arquitectura Serverless Zero-Build:** Funciona nativamente en cualquier navegador sin necesidad de Node.js, Webpack ni dependencias que compilar.

---

## 📂 Estructura Modular del Repositorio

```text
DidacticaEdInfantil/
│
├── index.html            # Maquetación semántica, cabecera, filtros, modales y enlaces
├── README.md             # Documentación pedagógica y técnica
├── .gitignore            # Exclusión de temporales de Office, Windows y editores
│
├── css/
│   └── styles.css        # Estilos visuales, animaciones, scrollbar y modo PDI
│
└── js/
    ├── data.js           # Catálogo de unidades y recursos con etiquetas pedagógicas
    ├── sheets.js         # Conexión con Google Sheets y exportaciones CSV/TSV
    └── app.js            # Lógica reactiva, filtros, favoritos, modales y búsqueda
```

---

## 🚀 Cómo Empezar

### Uso Inmediato en Local
1. Descarga o clona este repositorio.
2. Haz doble clic en el archivo [`index.html`](index.html).
3. ¡Listo! La aplicación se abrirá en cualquier navegador web moderno (Chrome, Edge, Firefox, Safari) sin requerir instalación de servidores.

---

## ☁️ Conexión con Google Sheets (Paso a Paso)

Si deseas gestionar y ampliar los recursos desde tu propia hoja de cálculo en la nube:

1. Entra en el **Modo Docente** pulsando el botón superior derecho (o pulsa `Ctrl + Mayús + D`).
2. Haz clic en **"Crear Google Sheet"** y copia la tabla o descarga el CSV para abrirlo en [Google Sheets](https://sheets.new).
3. En tu hoja de cálculo de Google Drive, pulsa **Compartir** y cambia los permisos a:  
   👉 **"Cualquier persona con el enlace"** con rol **Lector**.
4. Pulsa en **"Hoja en Vivo"** en el portal web y pega la URL de tu hoja de cálculo.
5. A partir de ese momento, cada fila que agregues a tu hoja se reflejará automáticamente en la web.

---

## 🌐 Publicación en GitHub Pages (Paso a Paso)

Este proyecto está 100% optimizado para publicarse de forma gratuita en **GitHub Pages**:

1. Crea un nuevo repositorio en tu cuenta de [GitHub](https://github.com) llamado `DidacticaEdInfantil`.
2. Sube la carpeta del proyecto (mediante **GitHub Desktop** o arrastrando los archivos a la web de GitHub).
3. En la página de tu repositorio en GitHub, ve a **Settings** > **Pages**.
4. En la sección **Build and deployment**:
   - **Source**: `Deploy from a branch`
   - **Branch**: Selecciona `main` (o `master`) y la carpeta `/ (root)`.
   - Haz clic en **Save**.
5. Tras unos 60 segundos, tendrás disponible la URL pública:  
   `https://<tu-usuario>.github.io/DidacticaEdInfantil/`

---

## 📄 Licencia y Uso Pedagógico

Desarrollado con fines educativos para la docencia en Formación Profesional. Libre para su adaptación, reutilización y mejora por la comunidad educativa.
