# Instructivo: Configuración de Chatbot con OpenAI API

## Descripción del Código

Este código crea un chatbot simple que utiliza la API de OpenAI (GPT-4o-mini) para mantener conversaciones con el usuario. El programa:

1. **Carga variables de entorno** desde un archivo `.env` para mantener segura la API key
2. **Inicializa el cliente de OpenAI** usando la API key
3. **Define una función de chat** que envía mensajes al modelo GPT-4o-mini
4. **Ejecuta un bucle interactivo** donde el usuario puede chatear con el bot

## Configuración Paso a Paso

### 1. Clonar o Crear el Repositorio

```bash
# Si es un proyecto nuevo
git init mi-chatbot-openai
cd mi-chatbot-openai

# Si clonas desde un repositorio existente
git clone <url-del-repositorio>
cd nombre-del-repositorio
```

### 2. Crear el Archivo Principal

Guarda el código en un archivo llamado `chatbot.py`:

```python
```

### 3. Obtener tu API Key de OpenAI

1. Ve a [platform.openai.com](https://platform.openai.com)
2. Inicia sesión o crea una cuenta
3. Navega a **API Keys** en el menú lateral
4. Haz clic en **"Create new secret key"**
5. Copia la API key (guárdala en un lugar seguro, no la podrás ver de nuevo)

### 4. Crear el Archivo de Variables de Entorno

Crea un archivo llamado `.env` en la raíz del proyecto:

```
OPENAI_API_KEY=tu-api-key-aqui
```

**¡IMPORTANTE!** Reemplaza `tu-api-key-aqui` con tu API key real de OpenAI.

### 5. Crear archivo .gitignore

Para mantener segura tu API key, crea un archivo `.gitignore`:

```
# Variables de entorno
.env

# Archivos de Python
__pycache__/
*.pyc
*.pyo
*.pyd
.Python

# Entornos virtuales
venv/
env/
ENV/

# IDEs
.vscode/
.idea/
*.swp
*.swo
```

### 6. Instalar Dependencias

Crea un archivo `requirements.txt`:

```
openai==1.35.3
python-dotenv==1.0.0
```

Luego instala las dependencias:

```bash
pip install -r requirements.txt
```

### 7. Configurar Git y Subir el Código

```bash
# Configurar Git (si es la primera vez)
git config --global user.name "Tu Nombre"
git config --global user.email "tu-email@ejemplo.com"

# Añadir archivos al repositorio
git add .

# Hacer el primer commit
git commit -m "Añadir chatbot con OpenAI API"

# Conectar con repositorio remoto (si aplica)
git remote add origin https://github.com/tu-usuario/tu-repositorio.git

# Subir los cambios
git push -u origin main
```

## Cómo Ejecutar el Programa

1. Asegúrate de tener instaladas las dependencias
2. Verifica que tu archivo `.env` contenga tu API key válida
3. Ejecuta el programa:

```bash
python chatbot.py
```

4. Comienza a chatear escribiendo mensajes
5. Para salir, escribe: `exit`, `quit` o `bye`

## Estructura del Proyecto

```
mi-chatbot-openai/
│
├── chatbot.py          # Código principal
├── .env                # Variables de entorno (NO SUBIR A GIT)
├── .gitignore          # Archivos a ignorar por Git
└── README.md           # Documentación (opcional)
```

## Notas Importantes

- **NUNCA** subas tu archivo `.env` a Git o repositorios públicos
- La API de OpenAI es de pago, monitorea tu uso
- El modelo `gpt-4o-mini` es más económico que `gpt-4`
- El rol debe ser `"system"` en lugar de `"developer"`
- Instala las dependencias necesarias (pip install openai python-dotenv)


```
