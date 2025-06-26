# CV Dinámico - Personalización

Este proyecto es una página web que muestra un currículum vitae de forma dinámica, cargando los datos desde un archivo JSON (`cv.json`). Puedes personalizar fácilmente la información para mostrar tu propio currículum.

## ¿Cómo personalizar tu CV?

### 1. Edita el archivo `cv.json`

Abre el archivo `cv.json` en la raíz del proyecto. Cambia los valores de los campos por tus propios datos. Por ejemplo:

```json
{
  "nombre": "Tu Nombre",
  "datosPersonales": {
    "nombre": "Tu Nombre Completo",
    "mail": "tu.email@ejemplo.com",
    "telefono": "+34 000 000 000",
    "direccion": "Tu Ciudad, País",
    "lema": "Tu lema personal o profesional",
    "fechaNacimiento": "YYYY-MM-DD"
  },
  "experiencia": [
    {
      "puesto": "Tu Puesto",
      "periodo": "Año de inicio - Año de fin",
      "descripcion": "Breve descripción del puesto",
      "funciones": [
        "Función 1",
        "Función 2"
      ]
    }
    // Puedes añadir más experiencias
  ],
  "formacion": [
    {
      "titulo": "Título o Grado",
      "horas": "Horas o créditos",
      "institucion": "Nombre de la institución",
      "temario": "Temas principales"
    }
    // Puedes añadir más formación
  ],
  "idiomas": [
    {
      "idioma": "Idioma",
      "lectura": 10,
      "escritura": 10,
      "comprension": 10,
      "nivel": "Nivel (A1-C2)"
    }
    // Puedes añadir más idiomas
  ],
  "habilidades": [
    {
      "nombre": "Habilidad",
      "nivel": 9
    }
    // Puedes añadir más habilidades
  ],
  "contacto": {
    "titulo": "Información de Contacto",
    "descripcion": "Texto de contacto"
  },
  "footer": {
    "texto": "© 2025 Tu Nombre"
  }
}
```

> **Nota:** No uses comentarios (`// ...`) dentro del JSON, ya que no son válidos y pueden causar errores.

### 2. Visualiza los cambios

Guarda el archivo y recarga la página `index.html` en tu navegador. Verás tu currículum actualizado automáticamente.

---

## Sugerencias de personalización avanzada

- **Añadir proyectos:**  
  Puedes ampliar el archivo `cv.json` añadiendo una sección de proyectos. Por ejemplo:

  ```json
  "proyectos": [
    {
      "nombre": "Nombre del Proyecto",
      "descripcion": "Descripción breve",
      "tecnologias": ["HTML", "CSS", "JavaScript"],
      "enlace": "https://enlace-al-proyecto.com"
    }
  ]
  ```

  Luego, añade una función en el JavaScript para mostrar esta sección en la página.

- **Agregar iconos SVG a habilidades:**  
  Puedes añadir un campo `svg` en cada habilidad para mostrar un icono personalizado.

- **Cambiar el estilo:**  
  Modifica los estilos en la etiqueta `<style>` de `index.html` para adaptar el diseño a tu gusto.

- **Soporte para más idiomas:**  
  Añade más campos o secciones si necesitas mostrar información en varios idiomas.

## Publicar tu CV en Netlify a través de GitHub

Puedes publicar fácilmente tu currículum en Netlify siguiendo estos pasos:

### 1. Sube tu proyecto a GitHub

1. Crea un nuevo repositorio en [GitHub](https://github.com/).
2. Sube todos los archivos de tu proyecto (incluyendo `index.html`, `cv.json`, etc.) al repositorio.






### 2. Conecta tu repositorio a Netlify

1. Ve a [Netlify](https://www.netlify.com/) y crea una cuenta si no tienes una.
2. Haz clic en **"Add new site"** y selecciona **"Import an existing project"**.
3. Elige **GitHub** como proveedor y autoriza a Netlify a acceder a tu cuenta.
4. Selecciona el repositorio donde subiste tu CV.
5. En la configuración, normalmente no necesitas cambiar nada si tu archivo principal es `index.html` en la raíz. Haz clic en **"Deploy site"**.

### 3. ¡Listo!

Netlify desplegará tu sitio y te dará una URL pública para compartir tu currículum online.

---

**Sugerencia:**  
Cada vez que actualices tu repositorio en GitHub, Netlify volverá a desplegar automáticamente tu sitio con los

---

¡Personaliza tu CV y hazlo único! Si tienes conocimientos de HTML y JavaScript, puedes seguir ampliando la funcionalidad según tus necesidades.