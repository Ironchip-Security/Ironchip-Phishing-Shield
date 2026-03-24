# Ironchip Phishing Shield

**Protección proactiva contra Typo-squatting, Ataques de Homógrafos y Phishing.**

<img width="705" height="605" alt="image" src="https://github.com/user-attachments/assets/e2d0a8a3-796b-4f8e-98bb-f49c4fa5c199" />

Bienvenido al repositorio de la extensión **Ironchip Phishing Shield**. 

Ironchip Phishing Shield es una extensión de navegador diseñada para proteger a usuarios y empleados de una de las amenazas más comunes en la web: el *phishing* (suplantación de identidad).

Utilizamos algoritmos de seguridad avanzados para detectar sitios maliciosos antes de que el navegador los cargue, evitando que ingreses credenciales o datos sensibles.

El repostorio contiene el instalador de la extensión y el fichero que alimenta la lista de dominios protegidos. Esta lista de dominios es de código abierto y colaborativa, crucial para la eficacia de la herramienta.

***

## ¿Qué hace exactamente?

1.  **Detección de Similitud (Typo-squatting):** Compara el dominio que estás visitando con nuestra **lista maestra** (alojada aquí) y tus **dominios personalizados**. Si un sitio como `gogle.com` se parece demasiado a uno legítimo (`google.com`), la extensión **bloquea la carga de la página** y te redirige a una pantalla de advertencia.
2.  **Detección de Homógrafos:** Identifica dominios que utilizan caracteres Unicode visualmente idénticos a letras latinas (ej. una 'a' cirílica en lugar de una 'a' normal) para engañar.
3.  **Análisis de Seguridad Externa (Opcional):** Si configuras tus claves API, realiza consultas en tiempo real a servicios de reputación como **VirusTotal** e **IPDB** para verificar si la URL o la IP de destino han sido reportadas como maliciosas.
4.  **Bloqueo de Formularios Maliciosos:** Si en una página legítima se detecta que un formulario intenta enviar tus credenciales a un dominio externo y no relacionado, la extensión te alerta inmediatamente.

***

## 💾 Instalación del Compilado (`.crx`)

Dado que esta extensión no está en la Chrome Web Store, la instalación debe realizarse a través del modo de desarrollador.

### ⚠️ Advertencia Importante

Chrome puede mostrar una advertencia al instalar extensiones fuera de la Chrome Web Store. El archivo compilado (`.crx`) en este repositorio ha sido firmado con nuestra clave.

### Pasos de Instalación:

1.  **Descargar el Archivo:**
    * Ve a la [pestaña principal del repositorio](https://github.com/Ironchip-Security/Ironchip-Phishing-Shield/tree/main).
    * Busca el archivo `Phishing Shield.crx` y descárgalo a tu ordenador.

2.  **Activar el Modo de Desarrollador en Chrome:**
    * Abre Google Chrome.
    * Navega a la página de extensiones escribiendo: `chrome://extensions/`
    * En la esquina superior derecha, activa el interruptor de **"Modo de desarrollador"** (Developer mode).

3.  **Instalar la Extensión:**
    * Localiza el archivo **`.crx`** que descargaste.
    * **Arrastra y suelta** el archivo **`.crx`** directamente sobre la página `chrome://extensions/`.
    * Chrome te pedirá una confirmación. Haz clic en **"Añadir extensión"**.

La extensión "Phishing Shield" se instalará y aparecerá en tu barra de herramientas.

***

## ⚙️ Primeros Pasos y Configuración de API Keys (Recomendado)

Para activar las funcionalidades, debes introducir tus claves de API en la página de opciones de la extensión. (Las que se te proporcionan en https://phishingshield.ironchip.com)

### 2. Configurar las Claves en la Extensión

Una vez que tengas tu clave:

1.  **Abrir Opciones:** Haz clic sobre el **icono de la extensión** ("Phishing Shield") en tu barra de Chrome.
2.  Se abrirá la página de configuración de la extensión.
3.  Introduce tu correo y la clave correspondientes.
4.  Haz clic en el botón **"Guardar"** (o el texto que hayas definido en tu página de opciones).

Una vez guardadas, la extensión comenzará a usar estos servicios para enriquecer su análisis y bloquear sitios basándose en la reputación de la comunidad de seguridad.

### Configuración (Recomendada)

Después de la instalación, haz clic en el icono de Ironchip y abre el *popup* para configurar la herramienta. La lista de **Dominios Personalizados** es fundamental para proteger activos internos de tu empresa.

***

## 🤝 Contribución y Actualización de Dominios

La lista de dominios base protegidos es la más amplia posible, y se mantiene de forma colaborativa a través de este repositorio.

***

*Desarrollado con pasión por la ciberseguridad en Ironchip.*
