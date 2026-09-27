# 📦 InventFast

> **Sistema web inteligente para la gestión y análisis de inventario**, desarrollado con Django y tecnologías de análisis de datos.

InventFast es una aplicación web diseñada para facilitar la administración de inventarios y transformar los datos registrados en información útil para apoyar la toma de decisiones.

Además de las funciones tradicionales de gestión, el sistema incorpora herramientas de **análisis, visualización y predicción** para identificar productos con alta o baja rotación y apoyar la planificación de reposición de stock.

---

## ✨ ¿Qué problema busca resolver?

La gestión de inventarios puede volverse complicada cuando la información se lleva de forma manual o se encuentra distribuida en diferentes registros.

Esto puede provocar:

* 📉 Dificultad para identificar productos con poca salida.
* 📦 Falta de control sobre los niveles de stock.
* ⚠️ Riesgo de quedarse sin productos importantes.
* 🔄 Reposición basada únicamente en observación o experiencia.
* 📊 Dificultad para interpretar el comportamiento histórico de las ventas.

**InventFast** busca centralizar esta información y utilizar los datos disponibles para proporcionar una visión más clara del estado del inventario.

---

## 🚀 Funcionalidades principales

### 📦 Gestión de inventario

* Registro y administración de productos.
* Control de entradas y salidas.
* Gestión de categorías.
* Gestión de marcas.
* Consulta del estado actual del inventario.
* Identificación de productos con stock bajo.

### 👥 Gestión del sistema

* Administración de usuarios.
* Registro de información relacionada con las operaciones.
* Gestión de facturas.

### 📊 Dashboard

El sistema incorpora un panel de información para visualizar de manera rápida el estado del inventario.

Incluye:

* Estadísticas generales.
* Indicadores de inventario.
* Gráficos.
* Comportamiento de productos.
* Información relevante para la toma de decisiones.

### 🤖 Análisis y funcionalidades inteligentes

Uno de los componentes principales de InventFast es el análisis de los datos históricos.

El sistema permite:

* 🔮 **Predecir productos con mayor probabilidad de venta.**
* 📉 **Detectar productos con baja rotación.**
* 📦 **Identificar necesidades de reposición.**
* 💡 **Generar recomendaciones relacionadas con el inventario.**
* 📈 Analizar tendencias mediante datos históricos.

> El objetivo de estas funcionalidades no es reemplazar la decisión del usuario, sino proporcionar información que facilite el análisis del inventario.

---

## 🖥️ Vista del sistema

> 📸 **Capturas de pantalla**

Aquí puedes colocar algunas imágenes del proyecto:

```text
📸 Dashboard
📸 Gestión de productos
📸 Inventario
📸 Análisis y predicciones
📸 Reportes
```

---

## 🛠️ Tecnologías utilizadas

### Backend

* 🐍 **Python**
* 🌐 **Django**

### Frontend

* HTML5
* CSS3
* JavaScript
* Tailwind CSS

### Análisis de datos e inteligencia

* 🐼 **Pandas**
* 🔢 **NumPy**
* 🧪 **SciPy**
* 🤖 **Scikit-learn**

### Visualización y generación de documentos

* 📊 **Chart.js**
* 📄 **WeasyPrint**
* 🖼️ **Pillow**

### Base de datos

* 🗄️ **SQLite**

---

## 🏗️ Arquitectura general

El proyecto sigue una estructura basada en Django, separando las diferentes responsabilidades de la aplicación.

```text
InventFast/
│
├── 📁 inventfast/
│   ├── settings.py
│   ├── urls.py
│   └── ...
│
├── 📁 apps/
│   ├── productos/
│   ├── inventario/
│   ├── facturas/
│   ├── usuarios/
│   └── ...
│
├── 📁 templates/
├── 📁 static/
├── 📁 media/
│
├── manage.py
├── requirements.txt
└── README.md
```

> *La estructura anterior es ilustrativa. Puedes ajustarla para que coincida exactamente con la estructura actual de tu repositorio.*

---

## ⚙️ Instalación y ejecución

### 1. Clonar el repositorio

```bash
git clone https://github.com/dmoinap/inventfast.git
```

### 2. Entrar al proyecto

```bash
cd InventFast
```

### 3. Crear un entorno virtual

```bash
python -m venv venv
```

Activarlo:

**Windows**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```

### 4. Instalar las dependencias

```bash
pip install -r requirements.txt
```

### 5. Ejecutar las migraciones

```bash
python manage.py migrate
```

### 6. Iniciar el servidor

```bash
python manage.py runserver
```

Luego abre:

```text
http://127.0.0.1:8000/
```

---

## 📈 Flujo general del sistema

```text
                 ┌──────────────────┐
                 │     Usuarios     │
                 └────────┬─────────┘
                          │
                          ▼
                 ┌──────────────────┐
                 │    InventFast    │
                 └────────┬─────────┘
                          │
             ┌────────────┼────────────┐
             ▼            ▼            ▼
        📦 Productos   🧾 Facturas   📊 Inventario
             │            │            │
             └────────────┼────────────┘
                          ▼
                  📊 Datos históricos
                          │
                          ▼
                 🤖 Análisis de datos
                          │
             ┌────────────┼────────────┐
             ▼            ▼            ▼
          🔮 Predicción  📉 Rotación  📦 Reposición
             │            │            │
             └────────────┼────────────┘
                          ▼
                   💡 Información
                  para decisiones
```

---

## 🎯 Objetivo del proyecto

El objetivo de InventFast es desarrollar una solución que combine la **gestión tradicional de inventario con herramientas de análisis de datos**, permitiendo que la información registrada pueda convertirse en indicadores y recomendaciones útiles.

De esta manera, el sistema no se limita únicamente a almacenar información, sino que busca **utilizar los datos para comprender el comportamiento del inventario**.

---

## 🧠 Conceptos aplicados

Durante el desarrollo se trabajaron conceptos relacionados con:

* Desarrollo web con Django.
* Arquitectura y organización de aplicaciones web.
* Modelado y gestión de bases de datos.
* Operaciones CRUD.
* Autenticación y gestión de usuarios.
* Procesamiento y análisis de datos.
* Visualización de información.
* Machine Learning.
* Predicción basada en datos históricos.
* Generación de reportes.
* Diseño de interfaces web.
* Validación y manejo de información.

---

## 🔮 Posibles mejoras

Algunas funcionalidades que podrían incorporarse en futuras versiones:

* [ ] Integración con PostgreSQL.
* [ ] Sistema de notificaciones.
* [ ] Predicciones con modelos más avanzados.
* [ ] Historial detallado de movimientos.
* [ ] Exportación de información en diferentes formatos.
* [ ] Gestión de múltiples sucursales.
* [ ] Sistema de roles y permisos más granular.
* [ ] Integración con proveedores.
* [ ] Mejoras en el análisis de tendencias.
* [ ] Despliegue en un servidor de producción.

---

## 📚 Contexto académico

**InventFast** fue desarrollado como proyecto académico dentro de la formación en **Ingeniería de Software**, aplicando conocimientos de desarrollo web, bases de datos, análisis de datos e inteligencia artificial.

El proyecto permitió integrar diferentes tecnologías en una aplicación funcional orientada a resolver un problema práctico de gestión.

---

## 👩‍💻 Autora

**Dyanne**

🎓 Estudiante de **Ingeniería de Software**

Interesada en el desarrollo de aplicaciones, análisis de datos, inteligencia artificial y creación de soluciones tecnológicas para problemas reales.

---

## ⭐ Proyecto

Si encuentras interesante el proyecto, puedes explorar el código fuente y conocer cómo fue construido.

**Tecnologías principales:**
`Python` · `Django` · `JavaScript` · `Tailwind CSS` · `Pandas` · `NumPy` · `Scikit-learn`

---
