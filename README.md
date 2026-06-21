<div align="center">

# Blog Personal con Jekyll

**Autor:** Alejandro De Mendoza  
**Asignatura:** Desarrollo de Aplicaciones en Red  
**Fecha:** 26 de octubre de 2025  
**Institución:** Universidad Internacional De La Rioja

</div>

---

---

## Descripción del Proyecto

Este proyecto consiste en la creación de un blog personal estático utilizando **Jekyll**, un generador de sitios web estáticos basado en Ruby. El blog aplica conceptos fundamentales de **HTML**, **CSS** y **Markdown** para la estructuración y diseño de contenido web.

El sitio incluye tres publicaciones sobre tecnología, desarrollo web e inteligencia artificial, además de páginas informativas como "Inicio", "Blog" y "Acerca de".

---

## Objetivos del Proyecto

1. Aplicar los fundamentos de HTML y CSS en un proyecto real.
2. Utilizar un generador de sitios estáticos (Jekyll) para construir un blog funcional.
3. Implementar un diseño responsivo y navegable.
4. Documentar el proceso de desarrollo de forma clara y profesional.

---

## Arquitectura del Proyecto

La estructura del proyecto sigue la convención estándar de Jekyll:

```
blog_alejandro/
├── _includes/
│   ├── footer.html          # Pie de página global
│   └── header.html          # Encabezado y menú de navegación
├── _layouts/
│   ├── default.html         # Plantilla base del sitio
│   └── post.html            # Plantilla para publicaciones individuales
├── _posts/
│   ├── 2025-10-26-introduccion-al-blog.md
│   ├── 2025-10-26-inteligencia-artificial-y-futuro.md
│   └── 2025-10-26-desarrollo-web-con-jekyll.md
├── assets/
│   └── css/
│       ├── style.scss       # Estilos del tema Cayman
│       └── custom.css       # Estilos personalizados
├── Imagenes/
│   ├── technologia.jpg
│   ├── artificial-intelligence.jpg
│   ├── creando_primer_blog_jekyll.jpg
│   ├── pagina_de_inicio.jpg
│   ├── acerca_de.jpg
│   └── blog.jpg
├── _config.yml              # Configuración principal de Jekyll
├── index.html               # Página de inicio
├── blog.md                  # Página de listado de publicaciones
├── about.md                 # Página "Acerca de"
├── Gemfile                  # Dependencias de Ruby
└── README.md                # Este archivo
```

---

## Tecnologías Utilizadas

- **Jekyll 4.4.1:** Generador de sitios estáticos.
- **Ruby 3.2.9:** Lenguaje de programación base.
- **HTML5:** Estructura semántica del contenido.
- **CSS3:** Diseño visual y responsivo.
- **Markdown:** Redacción de publicaciones.
- **Liquid:** Motor de plantillas de Jekyll.
- **Tema Cayman:** Tema visual base adaptado.

---

## Funcionalidades Implementadas

### 1. Páginas Principales

- **Inicio:** Página de bienvenida con listado de publicaciones recientes.
- **Blog:** Listado completo de todas las publicaciones con fechas.
- **Acerca de:** Información personal y objetivos del blog.

### 2. Publicaciones

Se crearon tres publicaciones con contenido extenso:

- **Introducción al Blog:** Presentación del propósito del sitio.
- **La Inteligencia Artificial y el Futuro:** Reflexión sobre el impacto de la IA.
- **Creando mi Primer Blog con Jekyll:** Experiencia personal de desarrollo.

Cada publicación incluye:

- Título y fecha de publicación.
- Imagen representativa.
- Contenido estructurado con subtítulos.
- Botones de navegación al final (volver al blog / volver al inicio).

### 3. Navegación

- Menú superior presente en todas las páginas con enlaces a Inicio, Blog y Acerca de.
- Botones de navegación contextuales en cada sección.
- Efecto hover en imágenes y botones para mejorar la interactividad.

### 4. Diseño Responsivo

- Las imágenes se ajustan automáticamente al ancho del contenedor.
- El diseño es compatible con dispositivos móviles y de escritorio.
- Uso de CSS Grid y Flexbox para el diseño de elementos.

---

## Instalación y Configuración

### Requisitos Previos

- **Ruby 3.2 o superior**
- **Bundler**
- **Jekyll 4.4.1**
- **Git** (opcional, para control de versiones)

### Instalación de Dependencias

#### 1. Instalar Ruby

En Windows:

```bash
winget install RubyInstallerTeam.Ruby.3.2
```

En macOS/Linux:

```bash
sudo apt-get install ruby-full
```

#### 2. Instalar Jekyll y Bundler

```bash
gem install jekyll bundler
```

#### 3. Verificar la instalación

```bash
ruby -v
jekyll -v
```

---

## Ejecución del Proyecto

### 1. Clonar o descargar el repositorio

```bash
git clone https://github.com/usuario/blog_alejandro.git
cd blog_alejandro
```

### 2. Instalar las dependencias del proyecto

```bash
bundle install
```

### 3. Ejecutar el servidor local

```bash
bundle exec jekyll serve
```

### 4. Abrir el navegador

Acceder a la siguiente URL:

```
http://127.0.0.1:4000/
```

El servidor se actualizará automáticamente al guardar cambios en los archivos.

---

## Abrir el Proyecto en Visual Studio Code

### Método 1: Desde la terminal

```bash
cd ruta/al/proyecto/blog_alejandro
code .
```

### Método 2: Desde VS Code

1. Abrir Visual Studio Code.
2. Ir a **Archivo → Abrir carpeta**.
3. Seleccionar la carpeta `blog_alejandro`.
4. Abrir una terminal integrada (**Ctrl + ñ** o **Ver → Terminal**).
5. Ejecutar `bundle exec jekyll serve`.

---

## Estructura de las Plantillas

### default.html

Plantilla base que define la estructura HTML general del sitio. Incluye:

- Declaración DOCTYPE.
- Enlaces a hojas de estilo (Cayman y custom.css).
- Inclusión del encabezado y pie de página.
- Contenedor principal para el contenido dinámico.

### post.html

Plantilla específica para las publicaciones individuales. Incluye:

- Título del post.
- Fecha de publicación.
- Imagen destacada (si existe).
- Contenido del post.
- Botones de navegación contextuales.

---

## Estilos Personalizados

Los estilos personalizados se encuentran en `assets/css/custom.css` e incluyen:

- Diseño de tarjetas para publicaciones.
- Estilos para imágenes con efecto hover.
- Botones de navegación con transiciones suaves.
- Diseño responsivo para diferentes tamaños de pantalla.
- Tipografía y espaciado optimizados para legibilidad.

---

## Configuración del Tema

El archivo `_config.yml` contiene la configuración principal del sitio:

```yaml
title: "Blog de Alejandro"
description: "Un espacio para aprender sobre desarrollo web e inteligencia artificial"
theme: jekyll-theme-cayman

plugins:
  - jekyll-feed

markdown: kramdown
```

---

## Publicación del Sitio

### Opción 1: GitHub Pages

1. Crear un repositorio en GitHub.
2. Subir el proyecto al repositorio.
3. Ir a **Settings → Pages**.
4. Seleccionar la rama `main` y la carpeta `/root`.
5. El sitio estará disponible en `https://usuario.github.io/blog_alejandro`.

### Opción 2: Netlify

1. Crear una cuenta en [Netlify](https://www.netlify.com/).
2. Conectar el repositorio de GitHub.
3. Configurar el comando de build: `jekyll build`.
4. Configurar el directorio de publicación: `_site`.
5. El sitio se publicará automáticamente.

---

## Comandos Útiles

| Comando                    | Descripción                           |
| -------------------------- | ------------------------------------- |
| `bundle exec jekyll serve` | Inicia el servidor local              |
| `bundle exec jekyll build` | Genera el sitio estático en `_site/`  |
| `bundle exec jekyll clean` | Limpia los archivos generados         |
| `bundle install`           | Instala las dependencias del proyecto |
| `gem update`               | Actualiza las gemas de Ruby           |

---

## Solución de Problemas Comunes

### Error: "jekyll command not found"

**Solución:** Asegurarse de que Ruby y Jekyll estén correctamente instalados y agregados al PATH del sistema.

```bash
gem install jekyll bundler
```

### Error: "Could not locate Gemfile"

**Solución:** Asegurarse de estar en el directorio raíz del proyecto donde se encuentra el archivo `Gemfile`.

```bash
cd blog_alejandro
```

### El servidor no se actualiza automáticamente

**Solución:** Reiniciar el servidor después de cambios en `_config.yml` o archivos en `_layouts/`.

```bash
bundle exec jekyll clean
bundle exec jekyll serve
```

---

## Créditos y Referencias

- **Jekyll Documentation:** [https://jekyllrb.com/docs/](https://jekyllrb.com/docs/)
- **Cayman Theme:** [https://github.com/pages-themes/cayman](https://github.com/pages-themes/cayman)
- **Markdown Guide:** [https://www.markdownguide.org/](https://www.markdownguide.org/)
- **Ruby Documentation:** [https://www.ruby-lang.org/en/documentation/](https://www.ruby-lang.org/en/documentation/)

---

## Licencia

Este proyecto fue desarrollado con fines académicos como parte de la asignatura **Desarrollo de Aplicaciones en Red**.

---

## Contacto

**Alejandro De Mendoza**  
Estudiante de Ingeniería Informática  
Email: alejandrotovarimpact@gmail.com  
GitHub: [AlejoTechEngineer](https://github.com/AlejoTechEngineer)

---

**Fecha de última actualización:** 26 de octubre de 2025
