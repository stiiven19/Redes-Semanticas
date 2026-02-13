# Redes Semánticas

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![NetBeans](https://img.shields.io/badge/NetBeans-1B6AC6?style=for-the-badge&logo=apache-netbeans-ide&logoColor=white)
![JGraphT](https://img.shields.io/badge/JGraphT-5E2CA5?style=for-the-badge&logo=graph&logoColor=white)
![GraphStream](https://img.shields.io/badge/GraphStream-00599C?style=for-the-badge&logo=graph&logoColor=white)

Este proyecto implementa un sistema de redes semánticas avanzado que permite modelar y manipular conocimiento a través de grafos. Las redes semánticas son una forma poderosa de representar el conocimiento mediante nodos (conceptos) y aristas (relaciones), permitiendo un análisis detallado de las conexiones entre conceptos.

## Características Principales

### Gestión de Grafos
- Creación y edición de grafos semánticos
- Visualización interactiva de redes con diferentes layouts
- Almacenamiento y carga de grafos en formato serializado
- Exportación e importación de grafos

### Análisis de Redes
- **Sistema de Activaciones**: Propagación de activaciones entre nodos para análisis de relevancia
- **Lista Jerárquica de Clases (LJC)**: Obtención de la jerarquía completa de clases para cualquier nodo
- **Búsqueda de Caminos**: Verificación de conexiones entre nodos y visualización de rutas
- **Análisis de Relaciones**: Identificación de patrones y conexiones entre conceptos

### Funcionalidades Avanzadas
- **Gestión de Anzuelos**: Marcado y seguimiento de nodos importantes
- **Parejas Semánticas**: Identificación de relaciones significativas entre conceptos
- **Análisis de Caminos**: Verificación de conexiones directas e indirectas
- **Sistema de Consultas**: Búsqueda avanzada en la red semántica

## Grafos de Ejemplo

El proyecto incluye un grafo de ejemplo que puedes cargar para probar la aplicación:

- **LJCevaluativo.ser** - Grafo de evaluación con jerarquía de clases que incluye ejemplos de relaciones semánticas y estructuras jerárquicas.

Para cargar un grafo:
1. Ve a `Archivo > Abrir`
2. Navega a la carpeta `grafos`
3. Selecciona el archivo .ser que desees cargar

## Estructura del Proyecto

```
RedesSemanticas/
├── src/                # Código fuente
├── lib/                # Bibliotecas necesarias
├── grafos/             # Grafos de ejemplo
│   └── LJCevaluativo.ser    # Grafo de ejemplo incluido
├── imagenes/           # Capturas de pantalla
│   ├── Grafo Graficado.png
│   └── Importando grafo.png
└── README.md           # Este archivo
```

## Requisitos

- Java 8 o superior
- Apache NetBeans (recomendado)
- Bibliotecas (incluidas en `/lib`):
  - JGraphT 1.5.2
  - GraphStream 2.0
  - Otras dependencias necesarias

## Guía de Uso

### Configuración Inicial
1. Clona el repositorio
2. Abre el proyecto en NetBeans
3. Asegúrate de que todas las bibliotecas en `/lib` estén correctamente configuradas
4. Ejecuta la clase principal `redessemanticas.RedesSemanticas`

### Cargar un Grafo de Ejemplo
1. Inicia la aplicación
2. Ve a `Archivo > Abrir`
3. Navega a la carpeta `grafos`
4. Selecciona un archivo .ser (por ejemplo, `LJCevaluativo.ser`)
5. Explora la red semántica cargada

### Crear un Nuevo Grafo
1. Ve a `Archivo > Nuevo`
2. Usa el botón derecho para agregar nodos
3. Conecta los nodos arrastrando entre ellos
4. Personaliza las propiedades de nodos y aristas
5. Guarda tu grafo con `Archivo > Guardar`

### Funciones Principales

### Panel de Información de Nodo

Al seleccionar cualquier nodo en el grafo, se muestra la siguiente información en el panel inferior:

1. **LJC (Lista Jerárquica de Clases)**: Muestra la jerarquía completa de clases del nodo seleccionado, permitiendo navegar a través de la estructura de herencia.

2. **Anzuelos**: Lista de nodos marcados como importantes (anzuelos) que están relacionados con el nodo seleccionado.

3. **Parejas**: Muestra las relaciones directas del nodo seleccionado con otros nodos, incluyendo el tipo de relación.

4. **Relaciones**: Lista todas las conexiones del nodo, mostrando tanto relaciones entrantes como salientes.

5. **Activaciones**: Muestra el nivel de activación actual del nodo y cómo se ha propagado a través de la red.

#### Cómo usar las funcionalidades:

1. **Selección de Nodos**:
   - Haz clic en cualquier nodo para ver su información detallada en el panel inferior
   - Usa Ctrl+clic para selección múltiple

2. **Gestión de Anzuelos**:
   - Haz clic derecho en un nodo y selecciona "Marcar como Anzuelo"
   - Los nodos anzuelo se resaltan en la visualización

3. **Exploración de Relaciones**:
   - Las relaciones se muestran automáticamente al seleccionar un nodo
   - Haz clic en cualquier relación para resaltar la conexión

4. **Navegación en la Jerarquía**:
   - Expande la sección LJC para ver la jerarquía completa
   - Haz clic en cualquier clase de la jerarquía para centrar la vista en ese nodo

## Capturas de Pantalla

### Interfaz Principal
![Interfaz Principal](imagenes/Grafo%20Graficado.png)

### Importando un Grafo
![Importando grafo](imagenes/Importando%20grafo.png)

## Notas
- Los archivos .ser contienen los grafos serializados
- Se recomienda no modificar manualmente los archivos en la carpeta `/lib`

## 👨‍💻 Desarrollado por

Steven Guerrero - Ingeniero de Sistemas  

