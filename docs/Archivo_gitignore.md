# **¿Que es .gitignore?**

Un .gitignore es un archivo de texto que le dice a Git qué archivos o carpetas NO debe seguir ni subir al repositorio.
Sirve para evitar subir cosas que:

 -Se generan automáticamente

 -Son específicas de tu máquina

 -Contienen información sensible

 -No aportan nada al código (basura, caché, etc.)

En resumen: mantiene tu repo limpio y profesional 😌

¿Qué se suele poner en un .gitignore para Python?  

🔹 1. Archivos de caché de Python

Python genera muchos archivos temporales que nunca deberías versionar:

__pycache__/
*.pyc
*.pyo
*.pyd

🔹 2. Entornos virtuales

Cada desarrollador tiene el suyo, así que no se suben:

venv/
.env/
.venv/
env/

🔹 3. Variables de entorno y secretos

Muy importante por seguridad 🔐:

.env
.env.local


(ahí suelen ir tokens, passwords, keys, etc.)

🔹 4. Archivos de IDEs y editores

Cosas de VS Code, PyCharm, etc.:

.vscode/
.idea/
*.swp

🔹 5. Logs y archivos temporales

No aportan nada al código:

*.log
*.tmp

🔹 6. Dependencias o builds (si aplica)

Por ejemplo, si usas packaging:

build/
dist/
*.egg-info/

