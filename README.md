
# Informe: Comandos básicos de Git y proceso para subir cambios a GitHub
**Autor:** Oscar Torres  Quintero
**Programa:** Analisis Y Desarrollo de software 
**Ficha:** 3293689
## 1. Resumen rápido — ¿Qué es Git y GitHub?
- **Git**: sistema de control de versiones distribuido que registra cambios en archivos y permite trabajar en equipo , la segunda importante de Linux Torvals (creador de Linux)
  -**GitHub**: servicio en la nube para alojar repositorios Git, colaborar, y mostrar proyectos
  ## 2. Proceso paso a paso para enviar tus cambios a GitHub![repositoriio]


A continuación presento el flujo típico, desde crear el repositorio remoto en GitHub hasta subir cambios desde nuestro equipo.

### Paso 1 — Crear el repositorio en GitHub
1. Entra a GitHub y crea un nuevo repositorio (en este caso mi respositorio tiene el nombre de "Git_comandos_informe").
2. Opcional: agrega un `README.md` desde la interfaz, o déjalo vacío.
3. (https://github.com/user-attachments/assets/b44a5621-cb5e-45cd-9e8a-4910cad0ad1e)
4. ### Paso 2 — Clonar el repositorio (o inicializar localmente)
5. ### Paso 2 — Clonar el repositorio (o inicializar localmente)
- Si creamos el repositorio  en GitHub y queremos trabajar localmente:

```bash
# clonar desde GitHub
git clone https://github.com/tu-usuario/mi-proyecto.git
cd mi-proyecto
```


- Si comienzas desde cero en tu máquina local:

```bash
mkdir mi-proyecto
cd mi-proyecto
git init
```
<img width="1536" height="1024" alt="CLONEGIT" src="https://github.com/user-attachments/assets/4f215600-1738-407c-ba86-9b82e277d081" />

### Paso 3 — Configurar usuario
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```![git1](https://github.com/user-attachments/assets/d11adae3-1b22-4ddb-8ab9-17a444b75bbb)
