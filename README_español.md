# 🤖 Bot de Propuestas Qubic

<div align="center">

### **Resúmenes Automáticos de Propuestas<br>para la Comunidad Qubic en 13 Idiomas**

<img width="250" height="250" alt="icon_2" src="https://github.com/user-attachments/assets/c960ae79-b84e-4b65-b540-360528faf126" />

</div>

## 📖 Tabla de Contenidos

- [🚀 Sobre el Proyecto](#-sobre-el-proyecto)
- [🏗️ Arquitectura & Tecnología](#️-arquitectura--tecnología)
- [📋 Idiomas Soportados](#-idiomas-soportados)
- [🎯 Funcionalidades en Detalle](#-funcionalidades-en-detalle)
- [💬 Uso en Discord](#-uso-en-discord)
  - [Añadir el Bot a tu Servidor](#añadir-el-bot-a-tu-servidor)
  - [Comandos de Discord](#comandos-de-discord)
- [📱 Uso en Telegram](#-uso-en-telegram)
  - [Añadir el Bot a tu Grupo](#añadir-el-bot-a-tu-grupo)
  - [Comandos de Telegram](#comandos-de-telegram)
- [⚙️ Gestión de Estado](#️-gestión-de-estado)
- [❓ Preguntas Frecuentes (FAQ)](#-preguntas-frecuentes-faq)
- [🛠️ Soporte](#️-soporte)

## 🚀 Sobre el Proyecto

El **Bot de Propuestas Qubic** es un bot desarrollado específicamente para la comunidad Qubic que detecta automáticamente nuevas propuestas de gobernanza, las resume usando IA en 13 idiomas diferentes y las publica en servidores de Discord y grupos de Telegram.

### 🌟 Beneficios Principales

- **🔍 Detección Automática** - Monitorea continuamente nuevas propuestas Qubic
- **🌍 Accesibilidad Multilingüe** - Hace las propuestas accesibles para miembros de la comunidad que no hablan inglés
- **🤖 Resúmenes con IA** - Utiliza DeepSeek AI para resúmenes precisos y fáciles de entender
- **⏰ Notificaciones Oportunas** - Publica nuevas propuestas en 15 minutos tras su publicación
- **📊 Resultados de Votación** - Publica automáticamente resultados al final de cada época

## 🏗️ Arquitectura & Tecnología

El bot está basado en una arquitectura multiplataforma robusta:

### Componentes Principales

- **Integración API Qubic** - Recupera propuestas activas y completadas
- **DeepSeek AI** - Crea resúmenes multilingües
- **Puentes Discord & Telegram** - Distribución multiplataforma
- **Almacenamiento en GitHub** - Gestión de estado persistente y caché
- **Caché Inteligente** - Evita llamadas API duplicadas

## 📋 Idiomas Soportados

El bot soporta actualmente **13 idiomas**:

| Idioma | Código |
|--------|--------|
| Alemán | `de` |
| Inglés | `en` |
| Francés | `fr` |
| Español | `es` |
| Italiano | `it` |
| Portugués | `pt` |
| Ruso | `ru` |
| Japonés | `ja` |
| Chino | `zh` |
| Coreano | `ko` |
| Árabe | `ar` |
| Turco | `tr` |
| Vietnamita | `vi` |

## 🎯 Funcionalidades en Detalle

### 🤖 Detección Automática de Propuestas
- **Intervalo de 15 Minutos** - Verifica regularmente nuevas propuestas
- **Procesamiento por Época** - Gestión de estado separada por época
- **Detección de Duplicados** - Previene notificaciones múltiples

### 🧠 Resúmenes de IA Inteligentes
- **Resumen Consciente del Contexto** - Extrae puntos clave de cada propuesta
- **Formateo Específico por Idioma** - Adaptado a matices culturales
- **Mecanismo de Caché** - Evita llamadas de IA duplicadas para las mismas propuestas

### 🔄 Gestión de Estado Robusta
- **Estado por Servidor/por Chat** - Cada comunidad gestiona su propio estado
- **Persistencia en GitHub** - Los estados sobreviven reinicios
- **Limpieza Automática** - Elimina datos de época obsoletos

### 🌐 Soporte Multiplataforma
- **Integración Perfecta en Discord** - Comandos slash y mensajes embed
- **Optimización para Telegram** - Teclados inline y soporte Markdown
- **Experiencia Consistente** - Mismas funcionalidades en ambas plataformas

## 💬 Uso en Discord

### Añadir el Bot a tu Servidor
1. Usa el [**enlace de invitación**](https://discord.com/oauth2/authorize?client_id=1400149716385267835&permissions=2147568640&integration_type=0&scope=applications.commands+bot)
2. Otorga **permisos de administrador** y añade el bot al canal deseado
3. Realiza la **configuración** con `/setup`

### Comandos de Discord

| **Comando** | **Descripción** | **Parámetros** |
|-------------|-----------------|----------------|
| ❔ `/help` | Mostrar ayuda | Ayuda detallada e instrucciones |
| ⚙️ `/setup` | Configura el bot para tu servidor | • `channel`: El canal para resúmenes de propuestas<br>• `language`: Idioma para los resúmenes |
| ℹ️ `/info` | Muestra información detallada del estado del bot | • Canal e idioma configurados<br>• Época actual<br>• Número de propuestas activas<br>• Estado de la API DeepSeek<br>• Tiempo de actividad del bot<br>• Intervalo de verificación |

## 📱 Uso en Telegram

### Añadir el Bot a tu Grupo
1. **Gestionar grupo**
2. **Añadir miembros**
3. **Buscar bot:** `@QubicTranslationBot`
4. **Añadir al grupo** como administrador
5. **Realizar configuración** en el chat deseado con `/setup`

> [!IMPORTANT]
> El comando `/setup` <ins>**debe**</ins> usarse en el chat donde se publicarán los resúmenes.

### Comandos de Telegram

| **Comando** | **Descripción** | **Parámetros** |
|-------------|-----------------|----------------|
| ❔ `/start` o `/help` | Mostrar ayuda | Ayuda detallada e instrucciones |
| ⚙️ `/setup` | Abre un teclado inline para selección de idioma | • Teclado inline con opciones de idioma<br>• Seleccionar idioma deseado |
| ℹ️ `/info` | Muestra información detallada del estado del bot | • Chat e idioma configurados<br>• Época actual<br>• Número de propuestas activas<br>• Estado de la API DeepSeek<br>• Tiempo de actividad del bot<br>• Intervalo de verificación |

## ⚙️ Gestión de Estado

El bot gestiona para cada época:

- **Propuestas Procesadas** - Evitación de duplicados
- **Contador de Propuestas** - Numeración continua por época
- **Estados Específicos por Idioma** - Permite cambiar idioma sin pérdida de datos

## ❓ Preguntas Frecuentes (FAQ)

### 🤔 Preguntas Generales

**P: ¿Qué idiomas están soportados?**  
R: Actualmente 13 idiomas: Alemán, Inglés, Francés, Español, Italiano, Portugués, Ruso, Japonés, Chino, Coreano, Árabe, Turco, Vietnamita.

**P: ¿Qué tan actualizados están los resúmenes de propuestas?**  
R: Las nuevas propuestas se detectan y resumen en 15 minutos tras su publicación.

**P: ¿Puedo cambiar el idioma después?**  
R: Sí, simplemente usa `/setup` nuevamente. Las propuestas ya procesadas se entregarán en el nuevo idioma.

### 🔧 Preguntas Técnicas

**P: El bot no responde a comandos - ¿qué hacer?**  
R: Asegúrate de que el bot tenga los permisos necesarios e intenta el comando nuevamente.

**P: ¿Cómo se anuncian los resultados de votación?**  
R: Cada miércoles a las 12:15 UTC, los resultados de la época anterior se publican automáticamente.

### 🌐 Preguntas Específicas por Plataforma

**P: ¿Funcionan todos los comandos en ambas plataformas?**  
R: Sí, la funcionalidad básica es idéntica en Discord y Telegram.

**P: ¿Puedo usar el bot tanto en Discord como en Telegram?**  
R: Sí, puedes usar el bot en ambas plataformas en paralelo.

**P: ¿Qué permisos necesita el bot en Discord?**  
R: El bot necesita permisos para enviar mensajes, integrar enlaces y usar comandos slash.

## 🛠️ Soporte

Para preguntas o problemas con el bot, por favor contacta a:

**📞 Contacto Discord/Telegram:** MDC

**⚠️ Importante:**  
Por favor asegúrate de tener la siguiente información lista:
- ID del servidor/chat donde ocurre el problema
- Comando exacto que no funciona
- Momento del problema
- Mensaje de error (si está disponible)

---

<div align="center">

**🤝 Un Proyecto para la Comunidad Qubic**  
*Haciendo las propuestas accesibles para todos, en todos los idiomas*

</div>
