# tarea3_servidor

# Tarea 3 - Gestión de Archivos PDF

## Descripción

Esta aplicación permite la carga y descarga de archivos PDF a través de un servidor Express con TypeScript. Los archivos se almacenan en la carpeta `documents` en la raíz del proyecto.

## Instalación

1. Clonar el repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd Tarea3
   ```

2. Instalar las dependencias:
   ```bash
   npm install
   ```

3. Iniciar el servidor:
   ```bash
   npm start
   ```

El servidor estará disponible en [http://localhost:3000](http://localhost:3000).

## Endpoints

### Subir Archivos PDF

- **POST** `/uploads`
- **Descripción:** Permite subir uno o varios archivos PDF.
- **Parámetro de cuerpo:** `docs` (Array de archivos PDF).

### Descargar Archivo

- **GET** `/download`
- **Descripción:** Permite descargar un archivo PDF.
- **Parámetro de consulta (query parameter):** `file` (nombre del archivo PDF).
  
Ejemplo:
   ```bash
   GET /download?file=nombre_archivo.pdf
   ```

## Notas

- Solo se aceptan archivos PDF para la carga.
- El servidor creará automáticamente la carpeta `documents` si no existe.

---

Asegúrate de completar estos puntos y tu proyecto debería estar listo para ser entregado.
