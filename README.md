# Dashboard de Equipos

Este proyecto es un dashboard interactivo que muestra información sobre equipos de desarrollo, sus integrantes y proyectos. Permite visualizar y comparar habilidades, certificaciones y el progreso de los proyectos.

## Características

- Visualización de equipos y sus integrantes
- Detalles de proyectos con seguimiento de progreso
- Comparación de habilidades entre equipos
- Estadísticas generales del equipo
- Interfaz responsive y moderna

## Estructura del Proyecto

```
team/
├── students.json      # Datos de estudiantes y equipos
├── teams-dashboard.html  # Interfaz del dashboard
├── package.json       # Configuración del proyecto
└── README.md         # Este archivo
```

## Requisitos

- Node.js (versión 14 o superior)
- NPM (incluido con Node.js)

## Instalación

1. Clona el repositorio:

```bash
git clone [URL_DEL_REPOSITORIO]
cd team
```

2. Instala las dependencias:

```bash
npm install
```

## Ejecución

1. Inicia el servidor de desarrollo:

```bash
npm start
```

2. Abre tu navegador y ve a:

```
http://localhost:8080/teams-dashboard.html
```

## Estructura de Datos

El archivo `students.json` contiene la siguiente estructura:

```json
{
  "metadata": {
    "version": "1.0.0",
    "lastUpdated": "2024-03-20",
    "description": "CRUI - PP3"
  },
  "students": [
    {
      "id": "STU001",
      "personalInfo": { ... },
      "academicInfo": { ... },
      "skills": { ... },
      "projects": [ ... ],
      "internships": [ ... ],
      "certifications": [ ... ],
      "languages": [ ... ]
    }
  ],
  "teams": [
    {
      "id": "TEAM001",
      "name": "Equipo 1",
      "members": ["STU001", "STU002"],
      "project": {
        "name": "Nombre del Proyecto",
        "description": "Descripción del proyecto",
        "technologies": ["React", "Node.js", ...],
        "status": "En desarrollo",
        "startDate": "2024-01-15",
        "expectedEndDate": "2024-07-15",
        "progress": 45
      }
    }
  ]
}
```

## Secciones del Dashboard

1. **Resumen General**

   - Total de equipos
   - Total de estudiantes
   - Total de skills
   - Total de certificaciones

2. **Equipos**

   - Información de integrantes
   - Skills por categoría
   - Certificaciones

3. **Proyectos**

   - Descripción detallada
   - Tecnologías utilizadas
   - Barra de progreso
   - Fechas de inicio y fin

4. **Comparación de Skills**
   - Tabla comparativa de habilidades
   - Visualización por equipo

## Personalización

Para modificar los datos:

1. Edita el archivo `students.json`
2. Mantén la estructura actual
3. Actualiza la página para ver los cambios

## Tecnologías Utilizadas

- HTML5
- CSS3
- JavaScript (ES6+)
- Bootstrap 5
- http-server (para desarrollo)

## Contribución

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.
