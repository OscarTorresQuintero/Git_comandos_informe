
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

- Si creamos el repositorio  en GitHub y queremos trabajar localmente:

```bash
# clonar desde GitHub
git clone https://github.com/tu-usuario/mi-proyecto.git
cd mi-proyecto
```

![git2](https://github.com/user-attachments/assets/fb8f031f-ac9a-4c34-ab00-e51983059333)

- Si comienzas desde cero en tu máquina local:

```bash
mkdir mi-proyecto
cd mi-proyecto
git init
```

### Paso 3 — Configurar usuario
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```

![git1](https://github.com/user-attachments/assets/d386f211-fdbf-4255-8735-03afaaa56ac6)
### Paso 4 — Crear o modificar archivos, revisar estado

```bash
# crear un archivo README o editar código
code README.md

# ver estado
git status
```
![readme](https://github.com/user-attachments/assets/7673add7-6514-47ef-9ed9-9f8743eeee14)

### Paso 5 — Añadir cambios al staging y commit

```bash
# añadir todos los cambios
git add .

# crear un commit con mensaje claro
git commit -m "Agrega informe sobre Git y GitHub"
```
![commit](https://github.com/user-attachments/assets/6173afdc-519e-4729-9e14-08b9a6d3521c)
### Paso 6 — Enlazar con el remoto (si no se clonó)


```bash
# sólo si no clonamos y no hay remoto aún
git remote add origin https://github.com/tu-usuario/mi-proyecto.git
```
### Paso 7 — Subir cambios al repositorio remoto

```bash
# si es la primera vez en la rama main (o master)
git push -u origin main

# para empujar en adelante
git push
```
![push](https://github.com/user-attachments/assets/1f7d4bd0-328f-447f-b1c2-b1d31048286d)

### Paso 8 — Verifica en GitHub
Entra a la página del repositorio en GitHub y confirma que tus archivos y commits aparecen.
![github](https://github.com/user-attachments/assets/2568bdb6-975c-4539-a09f-7003a3481f75)

## 3. Buenas prácticas y consejos

- Ignorar archivos innecesarios con `.gitignore` (node_modules/, .env, etc.).
- Crea ramas para nuevas funcionalidades: `git checkout -b feature/nueva-funcion`.
- Manténer commits pequeños y temáticos.
- Revisar `git pull` antes de empezar a trabajar para evitar conflictos.
- Cuando tengamos conflictos, resuélverlos localmente, probar y luego `git add` + `git commit`.
- Usar `git log --oneline --graph` para ver historial de forma gráfica en la terminal.

---

## 4. Estructura sugerida del repositorio
```
mi-proyecto/
├─ README.md
├─ screenshots/
│  ├─ 01_crear_repo_github.png
│  ├─ 02_clonar_repo.png
│  └─ ...
├─ src/
└─ .gitignore
```

---

## 5. Checklist de entrega
- [ ] README.md con explicación de comandos.
- [ ] Capturas de pantalla de cada paso en `screenshots/`.
- [ ] Repositorio público en GitHub.
- [ ] Enlace al repositorio incluido en la entrega.

---

## 6. Enlace de entrega 
https://github.com/OscarTorresQuintero/Git_comandos_informe






