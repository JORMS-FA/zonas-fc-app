# Zonas FC PRO 📊🚴🏃

**Zonas FC PRO** es una Progressive Web App (PWA) premium diseñada para ciclistas, corredores y atletas de resistencia que desean calcular sus zonas de entrenamiento de frecuencia cardíaca basándose de manera científica en su **Umbral de Lactato (LTHR)**, en lugar de fórmulas genéricas basadas en la frecuencia cardíaca máxima.

La aplicación unifica todas las versiones anteriores en una sola interfaz táctil, interactiva y móvil-primero con estética deportiva de alta gama.

---

## ✨ Características Principales

* **Guía Interactiva del Test de Friel**: Instrucciones paso a paso para realizar el test de campo contrarreloj de 20 minutos para estimar tu umbral de lactato con precisión.
* **Establecimiento Automatizado**: Permite ingresar tus ppm medias de los últimos 20 minutos de tu test y transferirlas instantáneamente a la calculadora.
* **Modelos Flexibles de Entrenamiento**:
  * **5 Zonas**: Estándar para ciclismo/running convencional.
  * **6 Zonas**: Diseñado para entrenamientos de alta intensidad (incluye zona específica de VO2 Máx).
* **Umbrales Fisiológicos Estimados**: Cálculo automático en tiempo real de tu primer umbral ventilatorio (**VT1**) y segundo umbral ventilatorio (**VT2** / Umbral Anaeróbico).
* **Gráfico HUD Deportivo**: Barra visual de segmentos de zonas coloreadas según los códigos de rendimiento deportivo estándar.
* **Historial Local (`LocalStorage`)**: Guarda tus resultados bajo títulos personalizados (ej. *Pretemporada 2026*, *Control de Verano*) con fecha y hora para observar tu progresión. Cárgalos o elimínalos en segundos.
* **Exportación a Imagen Premium (`html2canvas`)**: Genera una ficha gráfica nítida de alta resolución (`scale: 3`) lista para guardar en tu celular o compartir en redes sociales.
* **Progressive Web App (PWA)**: Soporte de instalación nativa y carga 100% offline mediante Service Workers, permitiendo usar la aplicación a pleno rendimiento en la montaña, carretera o zonas de nula cobertura móvil.

---

## 🛠️ Tecnologías Utilizadas

* **Estructura**: HTML5 Semántico.
* **Estilos**: CSS3 Moderno con variables personalizadas, efectos de desenfoque de cristal (Glassmorphism), transiciones aceleradas por hardware y diseño flexible (Flexbox y CSS Grid) responsivo para todo tipo de pantallas.
* **Lógica**: JavaScript ES6 puro, sin dependencias complejas.
* **Almacenamiento**: LocalStorage API del navegador.
* **Librerías externas**: `html2canvas.min.js` (cargada por CDN seguro) para la renderización impecable de la captura de pantalla.

---

## 🚀 Guía de Despliegue en GitHub Pages

Al ser una aplicación estática pura y libre de servidores (Serverless), se puede alojar de forma **100% gratuita** en GitHub Pages en menos de 3 minutos. Al alojarla en GitHub Pages, obtendrás un certificado de seguridad HTTPS automático, el cual es **indispensable** para que los navegadores registren y activen los Service Workers de la PWA.

Sigue estos sencillos pasos para desplegar tu aplicación:

### Paso 1: Crear un Repositorio en GitHub
1. Inicia sesión en tu cuenta de [GitHub](https://github.com/).
2. Haz clic en el botón **New** (Nuevo) para crear un nuevo repositorio.
3. Asígnale un nombre descriptivo, por ejemplo: `zonas-fc`.
4. Elige si quieres que sea Público o Privado (público es más fácil para Pages gratuito) y no inicialices con README, `.gitignore` ni licencia. Haz clic en **Create repository**.

### Paso 2: Inicializar Git y Subir los Archivos
Abre tu consola de comandos o Git Bash en la carpeta raíz del proyecto (`zonas-fc-app`) y ejecuta los siguientes comandos:

```bash
# 1. Inicializar el repositorio local
git init

# 2. Agregar todos los archivos al commit
git add .

# 3. Crear el primer commit
git commit -m "feat: version premium unificada de Zonas FC PRO"

# 4. Crear la rama principal llamada main
git branch -M main

# 5. Enlazar con tu repositorio remoto de GitHub
# (Reemplaza 'tu-usuario' por tu nombre de usuario de GitHub)
git remote add origin https://github.com/tu-usuario/zonas-fc.git

# 6. Subir tus archivos a GitHub
git push -u origin main
```

### Paso 3: Activar GitHub Pages en el Repositorio
1. En la página de tu repositorio en GitHub, ve a la pestaña ⚙️ **Settings** (Configuración) ubicada en el menú superior.
2. En la barra lateral izquierda, busca la sección **Code and automation** y haz clic en **Pages**.
3. En la sección **Build and deployment**:
   * En **Source**, asegúrate de que esté seleccionado **Deploy from a branch**.
   * Debajo de **Branch**, cambia el selector de `None` a **`main`**.
   * Deja la carpeta seleccionada como **`/ (root)`**.
4. Haz clic en el botón 💾 **Save** (Guardar).

### Paso 4: ¡Disfrutar de tu Web App!
GitHub comenzará a compilar y publicar tu sitio web de inmediato.
1. Espera aproximadamente 1 minuto.
2. Recarga la pestaña de configuración de Pages. Verás un banner destacado arriba que dice algo similar a:
   > 🚀 **Your site is live at** `https://tu-usuario.github.io/zonas-fc/`
3. Haz clic en el enlace para abrir tu aplicación. 
4. **Instalar en el Móvil**: Si entras desde tu celular (Safari en iOS usando "Compartir > Agregar a pantalla de inicio" o Chrome en Android usando los tres puntos > "Instalar aplicación"), la app se guardará en tu pantalla de inicio como una aplicación nativa.
