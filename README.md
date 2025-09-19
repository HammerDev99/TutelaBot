# TutelaBot 🧑‍⚖️📝

![Logo de TutelaBot](https://raw.githubusercontent.com/bladealex9848/TutelaBot/main/logo.png)

[![Version](https://img.shields.io/badge/versión-1.0.0-darkgreen.svg)](https://github.com/bladealex9848/TutelaBot)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.30.0-ff4b4b.svg)](https://streamlit.io/)
[![OpenAI](https://img.shields.io/badge/OpenAI_API-v2-00C244.svg)](https://platform.openai.com/)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-yellow.svg)](LICENSE)
[![Visitantes](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Ftutelabot.streamlit.app&label=Visitantes&labelColor=%235d5d5d&countColor=%231e7ebf&style=flat)](https://tutelabot.streamlit.app)

## 🧑‍⚖️ Descripción

TutelaBot es un asistente virtual especializado en los mecanismos constitucionales de protección de derechos fundamentales en Colombia: la **Acción de Tutela** y el **Derecho de Petición**, desarrollado con Streamlit y la API de OpenAI. Su base de conocimiento incluye la Constitución Política de Colombia de 1991, el Decreto 2591 de 1991 (que reglamenta la Acción de Tutela) y la Ley 1755 de 2015 (que regula el Derecho de Petición).

Este asistente está diseñado para proporcionar información clara y accesible sobre estos mecanismos fundamentales, ayudando a ciudadanos, abogados, estudiantes de derecho y funcionarios públicos a comprender su naturaleza, requisitos, procedimientos y plazos, facilitando así el acceso efectivo a la justicia y la protección de los derechos fundamentales en Colombia.

### 🍴 Fork del Proyecto Original

Este proyecto es un fork del trabajo original de **Alexander Oviedo Fadul**, adaptado y ajustado para necesidades específicas, incluyendo la configuración de API keys y Assistant ID personalizados para uso general.

## 🔍 Funcionalidades Principales

### 1. Acción de Tutela
- **Fundamento Constitucional y Legal**: Información sobre el artículo 86 de la Constitución y el Decreto 2591 de 1991
- **Derechos Protegidos**: Explicación detallada de los derechos fundamentales amparables vía tutela
- **Requisitos de Procedibilidad**: Orientación sobre subsidiariedad, inmediatez y demás requisitos
- **Legitimación**: Información sobre quién puede interponerla y contra quién procede
- **Procedimiento Completo**: Guía paso a paso desde la presentación hasta la revisión por la Corte Constitucional
- **Incidente de Desacato**: Explicación sobre qué hacer ante el incumplimiento de un fallo

### 2. Derecho de Petición
- **Fundamento Constitucional y Legal**: Información sobre el artículo 23 de la Constitución y la Ley 1755 de 2015
- **Modalidades**: Explicación de los diferentes tipos de peticiones y sus características
- **Términos y Plazos**: Detalle sobre los plazos legales para resolver cada tipo de petición
- **Requisitos de Presentación**: Orientación sobre el contenido mínimo y forma de presentación
- **Respuesta Adecuada**: Características que debe cumplir una respuesta de fondo
- **Silencio Administrativo**: Consecuencias de la falta de respuesta oportuna

### 3. Asistencia Práctica
- **Modelos y Ejemplos**: Plantillas y ejemplos adaptables para la redacción de documentos
- **Análisis de Casos**: Evaluación preliminar sobre la procedencia del mecanismo adecuado
- **Revisión de Documentos**: Análisis de borradores para sugerir mejoras
- **Orientación Procedimental**: Guía sobre autoridades competentes y trámites específicos
- **Referencias Normativas**: Citas precisas a artículos relevantes y jurisprudencia fundamental

### 4. Análisis de Documentos
- **Procesamiento de Texto**: Análisis de documentos legales como tutelas, peticiones o respuestas
- **Evaluación Jurídica**: Análisis preliminar desde la perspectiva constitucional y legal
- **Identificación de Elementos Clave**: Detección de aspectos relevantes o potenciales deficiencias
- **Sugerencias de Mejora**: Recomendaciones para fortalecer argumentos o corregir falencias

## 🚀 Instalación

### Requisitos Previos
- Python 3.8 o superior
- Pip (administrador de paquetes de Python)
- Cuenta en OpenAI con acceso a la API
- Asistente TutelaBot configurado en OpenAI

### Pasos de Instalación

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/bladealex9848/TutelaBot.git
   cd TutelaBot
   ```

2. **Crear un entorno virtual (recomendado)**
   ```bash
   python -m venv venv
   
   # En Windows
   venv\Scripts\activate
   
   # En macOS/Linux
   source venv/bin/activate
   ```

3. **Instalar las dependencias**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configurar credenciales**

   **Opción A: Usando variables de entorno**
   ```bash
   # En Windows
   set OPENAI_API_KEY=tu-api-key-aqui
   set ASSISTANT_ID=tu-assistant-id-aqui
   
   # En macOS/Linux
   export OPENAI_API_KEY=tu-api-key-aqui
   export ASSISTANT_ID=tu-assistant-id-aqui
   ```

   **Opción B: Usando archivo secrets.toml**
   
   Crea un archivo `.streamlit/secrets.toml` con el siguiente contenido:
   ```toml
   OPENAI_API_KEY = "tu-api-key-aqui"
   ASSISTANT_ID = "tu-assistant-id-aqui"
   ```

## ⚙️ Uso

### Iniciar la Aplicación

```bash
streamlit run app.py
```

Esto lanzará la aplicación y abrirá automáticamente una ventana del navegador en `http://localhost:8501`.

### Funcionalidades del Asistente

1. **Consultas Generales**
   - Pregunta sobre conceptos, procedimientos o normativa aplicable
   - Ejemplo: "¿Qué es una acción de tutela y cuándo procede?"

2. **Análisis de Casos**
   - Describe tu situación para recibir orientación sobre el mecanismo más adecuado
   - Ejemplo: "Mi EPS no me autoriza un medicamento urgente, ¿puedo usar tutela?"

3. **Solicitud de Formatos**
   - Pide modelos o ejemplos para redactar documentos según tu necesidad
   - Ejemplo: "Necesito un modelo de tutela contra mi EPS por negación de medicamentos"

4. **Revisión de Borradores**
   - Comparte tu borrador para recibir sugerencias de mejora
   - Ejemplo: "¿Puedes revisar este derecho de petición que redacté para mi universidad?"

5. **Información Procedimental**
   - Consulta sobre trámites, plazos, autoridades competentes o aspectos prácticos
   - Ejemplo: "¿Cómo puedo presentar una tutela de manera virtual?"

## ⚠️ Limitaciones

- TutelaBot proporciona información general y no constituye asesoría legal personalizada
- La información se basa en el conocimiento disponible hasta octubre de 2024
- Para casos específicos y complejos, siempre es recomendable consultar con un abogado
- El análisis de documentos es preliminar y no reemplaza la revisión profesional
- No puede garantizar resultados favorables en procesos judiciales o administrativos

## 📊 Escenarios de Uso

### 1. Ciudadanos
- Orientación sobre cómo proteger sus derechos fundamentales
- Ayuda para redactar correctamente tutelas y derechos de petición
- Información sobre plazos y procedimientos en lenguaje accesible

### 2. Abogados y Profesionales del Derecho
- Referencia rápida sobre normativa y jurisprudencia
- Revisión preliminar de documentos
- Modelos y plantillas para optimizar tiempo en la elaboración de documentos

### 3. Estudiantes de Derecho
- Apoyo para comprender conceptos y procedimientos
- Ejemplos prácticos para el aprendizaje
- Complemento para estudios sobre derecho constitucional y administrativo

### 4. Funcionarios Públicos
- Orientación sobre cómo responder adecuadamente a tutelas y derechos de petición
- Información sobre términos y requisitos legales
- Recursos para mejorar la calidad de las respuestas institucionales

## 👥 Contribuciones

Las contribuciones son bienvenidas. Para contribuir al desarrollo de TutelaBot:

1. Realiza un fork del repositorio
2. Crea una nueva rama (`git checkout -b feature/nueva-funcionalidad`)
3. Implementa tus cambios
4. Envía un pull request

## 📝 Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

## 🙏 Agradecimientos

- **OpenAI** por proporcionar la tecnología que impulsa el asistente
- **Streamlit** por facilitar el desarrollo de interfaces intuitivas
- **Corte Constitucional de Colombia** por su valioso desarrollo jurisprudencial
- **Comunidad jurídica colombiana** por su contribución al derecho constitucional

## 👤 Autores

### 🎯 Desarrollador Original
Creado con ❤️ por [Alexander Oviedo Fadul](https://github.com/bladealex9848)

[GitHub](https://github.com/bladealex9848) | [Website](https://alexanderoviedofadul.dev) | [LinkedIn](https://www.linkedin.com/in/alexander-oviedo-fadul/) | [Instagram](https://www.instagram.com/alexander.oviedo.fadul) | [Twitter](https://twitter.com/alexanderofadul) | [Facebook](https://www.facebook.com/alexanderof/) | [WhatsApp](https://api.whatsapp.com/send?phone=573015930519&text=Hola%20!Quiero%20conversar%20contigo!%20)

### 🍴 Adaptador del Fork
Adaptado y personalizado por [Daniel Arbeláez](https://github.com/HammerDev99) - Legal Tech Developer 🚀

[GitHub](https://github.com/HammerDev99) | [Website](http://portfolio.sprintjudicial.com/) | [Blog](https://blog.sprintjudicial.com/) | [LinkedIn](https://www.linkedin.com/in/daniel-arbelaez-/) | [Instagram](https://www.instagram.com/daniel_arbe99/) | [Twitter](https://x.com/hammerdev99) | [YouTube](http://youtube.com/@daainti/videos) | [Email](mailto:arbe.94@hotmail.com)

---

## 💼 Mensaje Final

TutelaBot busca democratizar el acceso a la información sobre los mecanismos constitucionales de protección de derechos fundamentales en Colombia, facilitando la comprensión de conceptos jurídicos complejos. Aunque este asistente proporciona información valiosa, recuerda que cada caso es único y puede requerir orientación profesional personalizada.

*"El conocimiento de los mecanismos constitucionales de protección es fundamental para garantizar el respeto de los derechos fundamentales y la construcción de una sociedad más justa e inclusiva."*