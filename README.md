# 🛡️ Ironchip Phishing Shield

**Protección proactiva contra Typo-squatting, Ataques de Homógrafos y Phishing de Servicios Corporativos.**

Bienvenido al repositorio que alimenta la lista de dominios protegidos de la extensión **Ironchip Phishing Shield**. Aunque el código de la extensión es propietario, esta lista de dominios es de código abierto y colaborativa, crucial para la eficacia de la herramienta.

***

## 💡 Sobre Ironchip Phishing Shield

Ironchip Phishing Shield es una extensión de navegador diseñada para proteger a usuarios y empleados de una de las amenazas más comunes en la web: el *phishing* (suplantación de identidad).

Utilizamos algoritmos de seguridad avanzados para detectar sitios maliciosos antes de que el navegador los cargue, evitando que ingreses credenciales o datos sensibles.

### ¿Qué hace exactamente?

1.  **Detección de Similitud (Typo-squatting):** Compara el dominio que estás visitando con nuestra **lista maestra** (alojada aquí) y tus **dominios personalizados**. Si un sitio como `gogle.com` se parece demasiado a uno legítimo (`google.com`), la extensión **bloquea la carga de la página** y te redirige a una pantalla de advertencia.
2.  **Detección de Homógrafos:** Identifica dominios que utilizan caracteres Unicode visualmente idénticos a letras latinas (ej. una 'a' cirílica en lugar de una 'a' normal) para engañar.
3.  **Análisis de Seguridad Externa (Opcional):** Si configuras tus claves API, realiza consultas en tiempo real a servicios de reputación como **VirusTotal** e **IPDB** para verificar si la URL o la IP de destino han sido reportadas como maliciosas.
4.  **Bloqueo de Formularios Maliciosos:** Si en una página legítima se detecta que un formulario intenta enviar tus credenciales a un dominio externo y no relacionado, la extensión te alerta inmediatamente.

***

## 🚀 Instalación y Primeros Pasos

La extensión debe instalarse como una extensión **desempaquetada** en navegadores basados en Chromium (Chrome, Edge, Brave, Opera).

### Instalación

1.  **Descarga el Archivo:** Obtén el archivo comprimido (`phishing_shield.zip`) proporcionado por Ironchip y **descomprímelo** en una carpeta local (ej. `C:\Extensiones\Ironchip`).
2.  **Abre la Gestión de Extensiones:** Ve a la URL de gestión de tu navegador: `chrome://extensions/`.
3.  **Modo Desarrollador:** Activa el **"Modo de desarrollador"** (Developer mode) en la esquina superior derecha.
4.  **Cargar Desempaquetada:** Haz clic en **"Cargar extensión sin empaquetar"** (Load unpacked) y selecciona la carpeta donde descomprimiste los archivos.

### Configuración (Recomendada)

Después de la instalación, haz clic en el icono de Ironchip y abre el *popup* para configurar la herramienta. La lista de **Dominios Personalizados** es fundamental para proteger activos internos de tu empresa.

***

## 🤝 Contribución y Actualización de Dominios

La lista de dominios base protegidos es la más amplia posible, y se mantiene de forma colaborativa a través de este repositorio.

### Archivo Maestro de Dominios

El archivo **`phishing_targets.txt`** contiene todos los dominios que la extensión utiliza para su comprobación de similitud. La extensión descarga automáticamente la versión más reciente de esta lista una vez cada **24 horas**.

**URL de Descarga (RAW):**
`[PEGA AQUÍ LA URL RAW DE TU FICHERO phishing_targets.txt]` 

### Cómo Añadir/Sugerir un Dominio

Si un dominio de alto valor para ti o tu empresa no está en la lista:

1.  **Haz un Fork** de este repositorio.
2.  **Edita el archivo `phishing_targets.txt`**.
3.  Añade el dominio que deseas proteger en una nueva línea, **sin el prefijo `www.`** y en **minúsculas**.
    * *Ejemplo de línea:* `mi-banco-corporativo.com`
4.  **Crea un Pull Request (PR)**.
5.  El equipo de Ironchip revisará y fusionará los cambios. Los usuarios de la extensión recibirán la actualización automáticamente en su siguiente ciclo de descarga (máximo 7 dias).

***

## 🔮 Roadmap Futuro (Próximas Mejoras)

Estamos trabajando continuamente para mejorar la eficacia de la protección de Ironchip:

* **Integración con Machine Learning:** Uso de modelos para clasificar la legitimidad de una página basándose en el diseño, contenido y metadatos, no solo en la URL.
* **Análisis de Certificados:** Detección de certificados SSL recién emitidos o con datos sospechosos.
* **Gestión Centralizada de Políticas:** Para clientes corporativos, la capacidad de desplegar la lista de dominios personalizados y claves API de forma remota a todos los empleados.
* **Soporte Multi-Navegador:** Lanzamiento oficial en la tienda de extensiones de Firefox.

***

*Desarrollado con pasión por la ciberseguridad en Ironchip.*
