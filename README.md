[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/C6PSew_P)
# Unidad No. 1 - Git y GitHub
## Información del estudiante  
Nombre del estudiante:  
Id.:  
---
# Evaluación

### **Descripción de la Actividad:**

Vas a clonar el repositorio en tu computador. Posteriormente, vas a crear una serie de carpetas y archivos, tal como se describe en las **Instrucciones**. En cada uno de los pasos que realices, debes crear un **commit** (en total, deben ser más de 10). Incluye imágenes, pantallazos y todo lo que consideres necesario para que tu repositorio esté organizado y se entienda. El aspecto visual es importante. Debes utilizar el lenguaje **Markdonw** para mejorar la presentación de tu proyecto.


## Instrucciones:

1. **Crea la estructura del proyecto:**
    - Clona el repositorio de la evaluación.
    - De ahora en adelante seguirás trabajando en tu repositorio local.
    - Ubícate en el directorio raíz llamado `prog-Eval_Template`.
    - Dentro de este directorio, crea las siguientes carpetas:
        - `src`: para almacenar el código fuente.
        - `docs`: para guardar la documentación.
        - `images`: para imágenes relacionadas con el proyecto.

2. **Código fuente:**
    - En la carpeta `src`, crea un script en Python (ej. script.py) con el siguiente código:
        
        ```python
        # Programa para calcular el promedio de una lista de números
        
        print("Bienvenido al programa de cálculo de promedios.")
        print("Ingresa números uno por uno. Escribe 'salir' para terminar.")
        
        # Lista para almacenar los números
        numeros = []
        
        while True:
            entrada = input("Ingresa un número (o escribe 'salir'): ")
            
            if entrada.lower() == 'salir':
                break  # Salir del bucle si el usuario escribe 'salir'
            
            try:
                # Convertir la entrada a número
                numero = float(entrada)
                numeros.append(numero)
            except ValueError:
                print("Por favor, ingresa un número válido.")
                continue
        
        # Verificar si hay números en la lista antes de calcular el promedio
        if len(numeros) > 0:
            promedio = sum(numeros) / len(numeros)
            print(f"El promedio de los números ingresados es: {promedio:.2f}")
        else:
            print("No ingresaste ningún número.")
        
        ```
        
    - Este código es solo un ejemplo básico para incluir un archivo funcional en el proyecto.
    
3. **Archivo .gitignore:**
    
    Investiga qué es un archivo `.gitignore` y para qué se utiliza en un proyecto de programación. Guarda el resultado de tu consulta en la carpeta `docs`, en un documento llamado `Archivo_gitignore.md`. Posteriormente, crea el archivo `.gitignore` y guárdalo en tu repositorio (afuera de todo). Ahora, según la consulta que hiciste, escribe en él los nombres de archivos y carpetas que quieres ignorar. Pregunta al profesor tus dudas.
    
4. **Documentación:**
    - Dentro de la carpeta `docs`, crea los siguientes archivos de tipo Markdown (.md):
        - `uso_consola.md`: Describe los conceptos aprendidos sobre cómo usar la consola para navegar y crear directorios y archivos. Haz un listado de los principales comandos utilizados en esta unidad. Agrega pantallazos de algunos comandos para complementar tu explicación.
        - `repositorio_local.md`: Explica cómo crear un repositorio local con comandos de Git.
        - `repositorio_remoto.md`: Detalla el proceso para crear un repositorio remoto en GitHub y sincronizarlo con el repositorio local.
5. **Archivo README.md:**
    - En la raíz del proyecto encontrarás un archivo `README.md`, es este mismo que estás leyendo. Lo vas a editar y vas a incluir al inicio del archivo la siguiente información:
        - Una breve descripción del contenido de tu repositorio. Recuerda que los archivos README.md están ahí para explicar a las personas que vean tu repositorio, de qué se trata y qué contiene.
        - Explica los pasos necesarios para clonar y ejecutar el proyecto.
        - Crea una tabla de contenido con enlaces a los archivos Markdown de la carpeta `docs`.
6. **Uso de Git:**
    - Realiza un **commit** para cada etapa del desarrollo (creación de carpetas, scripts, archivos Markdown, etc.). **Debes realizar mínimo 10 commits.** Los mensajes que utilices deben ser claros, con buena ortografía y con información relevante sobre el cambio que acabas de realizar.
    - Asegúrate de incluir imágenes con pantallazos de los pasos que realices cuando añadas elementos a tu repositorio y de los comandos de Git que utilices y su resultado.
    - Recuerda que los archivos son de Markdown; por lo tanto, debes utilizar los comandos correctos para que se visualicen correctamente.
7. **Entrega:**
    - Sube los cambios de tu proyecto al repositorio remoto de GitHub.
    - Asegúrate de que toda la documentación esté completa y correctamente estructurada.
