# 1. Intento inicial de creación de cuenta (Simulación de error y solución)
echo "Error detectado: El correo anterior ya estaba vinculado o bloqueado."
echo "Solución: Creando nueva cuenta de GitHub con correo alternativo..."

# 2. Configuración de identidad local (Post-creación de cuenta exitosa)
git config --global user.name "TuNombreUsuario"
git config --global user.email "tu-nuevo-email@ejemplo.com"

# 3. Instalación de Cursor IDE
# Si estás en Windows, Claude te sugeriría descargar el .exe
brew install --cask cursor

# 4. Inicialización del Repositorio
mkdir mi-nuevo-proyecto
cd mi-nuevo-proyecto
git init
touch README.md
echo "# Mi Proyecto con Cursor y Claude" >> README.md
git add .
git commit -m "Initial commit: Configuración de entorno"

# 5. Instrucción para Claude Code sobre extensiones:
# "Claude, por favor abre Cursor y guía la instalación de los plugins 'Claude Code' y 'Codex'"
cursor .
