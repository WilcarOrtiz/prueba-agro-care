# 🌾 AgroCare - Guía Completa de Instalación y Uso

## Para Principiantes - ¡Explicado en Términos Simples!

---

## 📖 ¿QUÉ ES AGROCARE?

**AgroCare** es una aplicación de escritorio (un programa que instalas en tu computadora) que te ayuda a **gestionar tu granja o campo agrícola**.

🌐 Documentación Online

Puedes ver la explicación completa y guía visual aquí:
👉 https://agro-care-explicacion-gi6t.vercel.app/
Piensa en él como una **libreta digital inteligente** donde puedes:

* 📝 Registrar información sobre tus cultivos
* 📊 Ver datos y estadísticas
* 💾 Guardar toda la información de forma segura
* 🖥️ Acceder fácilmente desde tu computadora

**Es similar a:** Excel, pero especializado para agricultura y más fácil de usar.

---

## 🎯 ANTES DE EMPEZAR - REQUISITOS

### 📦 Tecnologías que usa AgroCare

AgroCare utiliza varias herramientas importantes:

* **JavaFX** → Para crear la interfaz gráfica
* **Scene Builder** → Para diseñar las pantallas visualmente sin escribir tanto código
* **GSON** → Para convertir datos entre Java y formato JSON (lectura/escritura de datos)

Esto significa que podrás modificar las ventanas con Scene Builder y manejar datos fácilmente con GSON.

Antes de instalar AgroCare, tu computadora necesita tener ciertos "programas base" instalados. Son como los **cimientos de una casa** - sin ellos, el programa no puede funcionar.

### ¿QUÉ NECESITAS INSTALAR?

1. **Java (JDK 21)** - El "idioma" que entiende AgroCare
2. **JavaFX (21 SDK)** - Los "colores y botones" del programa
3. **Git** (opcional) - Para descargar el proyecto

### VERIFICAR SI YA LO TIENES INSTALADO

#### Paso 1: Abre la Terminal/Símbolo del Sistema

**En Windows:**

* Presiona `Windows + R`
* Escribe `cmd` y presiona Enter
* Se abrirá una ventana negra

**En Mac:**

* Presiona `Cmd + Espacio`
* Escribe `Terminal` y presiona Enter

**En Linux:**

* Abre la aplicación "Terminal"

#### Paso 2: Verifica si Java está instalado

Copia y pega esto en la terminal:

```bash
java -version
```

**Si ves algo como esto: ✅ YA TIENES JAVA**

```plaintext
java version "21.0.8" 2024-04-16 LTS
```

**Si ves un error como "comando no encontrado": ❌ NECESITAS INSTALAR JAVA**

---

## INSTALACIÓN PASO A PASO

### PASO 1: INSTALAR JAVA JDK 21

Java es el "motor" que hace funcionar AgroCare.

#### Para Windows:

1. Ve a la página oficial de descargas de Oracle Java
2. Haz clic en **"Java 21"** (o versión más reciente)
3. Bajo "Windows x64 Installer", descarga el archivo `.exe`
4. Ábrelo
5. Haz clic en **"Next"**, luego **"Install"**
6. Espera unos minutos
7. Cierra el instalador

**Verificar instalación:**

```shell
java -version
```

Si ves la versión 21 → ¡Java está instalado! 🎉

#### Para Mac:

* Descarga Java 21 para macOS
* Abre el archivo `.dmg`
* Instala normalmente

#### Para Linux (Ubuntu/Debian):

```shell
sudo apt update
sudo apt install openjdk-21-jdk
```

---

### PASO 2: INSTALAR JAVAFX 21 SDK

JavaFX es lo que permite que AgroCare tenga ventanas, botones y diseño visual.

#### Funciona igual en Windows, Mac y Linux:

1. Descarga **JavaFX 21 SDK** desde la página oficial de Gluon
2. Extrae el `.zip`
3. Guarda la carpeta en una ruta fácil de recordar

Ejemplos de rutas recomendadas:

* Windows: `C:\Program Files\Java\javafx-sdk-21.0.8`
* Mac: `/Users/tuusuario/javafx-sdk-21.0.8`
* Linux: `/home/tuusuario/javafx-sdk-21.0.8`

**IMPORTANTE:** Necesitarás esta ruta luego.

---

## PASO 3: DESCARGAR EL PROYECTO AGROCARE

### OPCIÓN A (Fácil): Descargar ZIP

1. Entra al repositorio del proyecto
2. Haz clic en el botón verde **"Code"**
3. Selecciona **"Download ZIP"**
4. Extrae el archivo
5. Mueve la carpeta a un lugar cómodo (`C:\AgroCare` por ejemplo)

### OPCIÓN B (Avanzada): Usar Git

```shell
git clone https://github.com/WilcarOrtiz/prueba-agro-care.git
cd prueba-agro-care
```

---

# 🚀 EJECUTAR AGROCARE

## OPCIÓN 1: Usar NetBeans (Recomendado)

### Paso 1: Instalar NetBeans

* Descárgalo desde la página oficial
* Instálalo normalmente

### Paso 2: Abrir el proyecto

1. Abre NetBeans
2. Ve a **File → Open Project**
3. Selecciona la carpeta del proyecto
4. Haz clic en **Open**

### Paso 3: Configurar JavaFX

1. Clic derecho en el proyecto → **Properties**
2. Ve a **Build → Compile**
3. En **Javac Options**, pega:

Windows:

```plaintext
--module-path "C:\Program Files\Java\javafx-sdk-21.0.8\lib" --add-modules javafx.controls,javafx.fxml
```

Mac:

```plaintext
--module-path "/Users/tuusuario/javafx-sdk-21.0.8/lib" --add-modules javafx.controls,javafx.fxml
```

Linux:

```plaintext
--module-path "/home/tuusuario/javafx-sdk-21.0.8/lib" --add-modules javafx.controls,javafx.fxml
```

4. Guardar

### Paso 4: Ejecutar AgroCare

* Presiona **F6** o haz clic en el botón verde "Play"
* Espera unos segundos
* ¡Listo! Se abrirá AgroCare 🎉

---
