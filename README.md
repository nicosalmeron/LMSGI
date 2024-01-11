# Cuaderno lenguaje de marcas
# Tabla de contenidos
## Enlaces de interés
* [W3](https://www.w3.org/)

## Qué es un Lenguaje de marcas
Es un lenguaje escrito usando caracteres especiales y texto legible para los humanos. El texto es interpretado por un software especifico (normalmente un navegador web) para luego mostrarlo en un formato específico el cual es dado por cómo se ha escrito el texto usando el lenguaje de marcas, por ejemplo, ahora que estoy usando Markdown, si escribo una palabra entre dos asteriscos (** xxxxx **) a cada lado se verá en negrita: **prueba**
## Evolución de los lenguajes de marcas
- SGML
Se trata de un metalenguaje, se usa como base para la creación de otros lenguajes de marcado como HTML y XML.

- GML
Es un lenguaje creado con el propósito de mostrar información cartográfica en aplicaciones especificas sobre la geografía

## Características de los lenguajes de marcas
**No son lenguajes de programación**, se tratan de lenguajes para la visualización de contenido. La escritura de estos lenguajes es legible para los humanos ya que se usan palabras, pero cada lenguaje de marcas tiene su sintáxis específica además de una estructura jerárquica para organizar el contenido. Estos lenguajes son usados en la gran mayoría de aplicaciones gracias a su flexibilidad y adaptabilidad a cada situación en especifico.

## Características y ejemplos de los siguientes lenguajes de marcas
- XML
  
Se trata de un lenguaje de marcas usado para almacenar y mostrar información de manera legible tanto para un ordenador como para un ser humano. Cuenta con las bases de un lenguaje de marcado (como la estructura jerárquica, el uso de marcas para el contenido o los atributos) y con características diferenciadoras como lo es el esquema XML que nos permite especificar las reglas y la estructura válida en nuestro documento. Un ejemplo de este tipo de lenguaje de marcas sería el siguiente:

```
<?xml version="1.0" encoding="UTF-8"?>
<coche marca="Toyota" modelo="Corolla">
    <descripcion>
        <color>Rojo</color>
        <año>2022</año>
        <precio moneda="USD">20000</precio>
    </descripcion>
    <caracteristicas>
        <motor tipo="Gasolina">1.8L</motor>
        <transmision>Automática</transmision>
</coche>

```

- HTML
  
Un lenguaje enfocado a la web y a la presentación de contenido. Con él podremos añadir enlaces, multimedia, formularios y una infinidad de posibilidades con sus atributos. También podremos darle formato al texto sin necesidad de usar CSS ya que tambien tiene atributos dedicados a esto, como `style`. He aquí un ejemplo de un código HTML:

```
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo HTML</title>
</head>
<body>
    <h1>¡Hola, mundo!</h1>
    <p>Esto es un HTML de ejemplo.</p>
</body>
</html>

```

- JSON
  
Está destinado al intercambio de datos entre una aplicación y un servicio web. Utiliza una sintáxis simple basada en "clave-valor" cada línea separada por comas y resulta legible para el ojo humano. Tiene una estructura anidada y jerárquica, lo que significa que un objeto JSON puede contener otros objetos JSON y cada clave puede contener más de un valor:

```
{
    "libros": [
        {
            "titulo": "El Gran Gatsby",
            "autor": "F. Scott Fitzgerald",
            "publicacion": 1925,
            "genero": "Novela"
        },
        {
            "titulo": "Cien años de soledad",
            "autor": "Gabriel García Márquez",
            "publicacion": 1967,
            "genero": "Novela"
        },
    ]
}

```

- YAML
  
Un lenguaje destinado especialmente a archivos de configuración escritos de manera sencilla y entendible. Se suelen hacer anotaciones dentro del archivo y se caracteriza tambien por las referecias, lo que nos permite la reutilización de un dato sin tener que escribirlo, evitando así la duplicación de este. Aqui dejo un ejemplo de YAML:

```
#Let NetworkManager manage all devices on this system
network:
  version: 2
  renderer: NetworkManager
  ethernets:
   enp0s3:
    dhcp4: no
    addresses
    - 192.168.0.80/24
    gateway4: 192.168.0.1
    nameserver:
     addresses: [192.168.0.20]

```
  
## XML: definición y características del metalenguaje
- Prologo

Se trata de una línea opcional al inicio del archivo XML, la cual indica ciertos parámetros sobre el archivo. El prólogo, por lo general, incluye lo siguiente:

```
<?xml version="1.0" encoding="utf-8" standalone="no"?>

```
Comienza con `<?xml version=""` que indica la versión que se está usando, luego `encoding=""` que nos indica que codificación de caracteres se está usando (lo más usual es UTF-8 ya que admite todos los caracteres alfanuméricos) y por último `standalone="">` lo cual se usa para la validación del documento.

- Contenido

El contenido está comprendido entre una etiqueta raíz la cual marcará el inicio y el fin de este. El contenido debre estar marcado por etiquetas y sus atributos si se precisa de ellos de manera que el cuerpo del archivo quedaría tal que así:
```
<raiz>
  <colores>
    <color>Rojo</color>
    <color>Verde</color>
    <color>Azul</color>
  </colores>
</raiz>

```
- Atributos

Los atributos son valores que se encuentran dentro de las etiquetas. Se usan para añadir información a el valor y optimizar el espacio en el documento. Muchas veces también nos resulta más facil la lectura si los valores del objeto los dividimos entre atributos y el cuerpo del objeto. Se ven tal que así:

```ruby
<persona nombre="Juan" edad="30" genero="Masculino" />

```
- Ejemplos en XML

Por lo tanto, un archivo XML completo quedaría tal que así:
```ruby
<?xml version="1.0" encoding="UTF-8"?>
<root>
    <cancion id="1" genero="alternativo">
        <titulo>Video Games</titulo>
        <album>Born to Die</album>
        <año>2011</año>
    </cancion>
    <cancion id="2" genero="alternativo">
        <titulo>Religion</titulo>
        <album>Honeymoon</album>
        <año>2015</año>
    </cancion>
    <cancion id="3" genero="blues rock">
        <titulo>Shades of Cool</titulo>
        <album>Ultraviolence</album>
        <año>2014</año>
    </cancion>
</root>
```

## Sistemas de gestión de información
Sus características incluyen almacenamiento estructurado, acceso y recuperación de información, seguridad, integración de datos, automatización de procesos, interfaz de usuario intuitiva, escalabilidad, auditabilidad, respaldo y recuperación, personalización, colaboración, y herramientas para informes y análisis. Estas funciones mejoran la eficiencia en la toma de decisiones y en la administración de recursos de información en una organización.

- Sistemas de Gestión de Bases de Datos (SGBD)
- Sistemas de Gestión de Documentos (DMS)
- Sistemas de Gestión de Contenido (CMS)
- Sistemas de Información Geográfica (SIG)
- Sistemas de Gestión de Recursos Empresariales (ERP)
- Sistemas de Gestión de Relaciones con el Cliente (CRM)
- Sistemas de Gestión de Proyectos (PMS)

## ERP (Enterprise Resource Planning)
**Características del ERP:**
- *Integración:* Unifica datos y procesos.
- *Módulos Funcionales:* Adaptados a áreas específicas.
- *Automatización:* Mejora la eficiencia y reduce errores.
- *Colaboración:* Facilita la comunicación interna.
- *Informes y Análisis:* Toma decisiones basadas en datos.

**Beneficios del ERP:**
- *Eficiencia Operativa:* Optimiza procesos y reduce redundancias.
- *Toma de Decisiones Informada:* Ofrece información en tiempo real.
- *Reducción de Costos:* Minimiza costos operativos.
- *Mejora en la Productividad:* Libera tiempo para tareas estratégicas.
- *Mejora en la Atención al Cliente:* Facilita seguimiento y gestión eficiente.
- *Competitividad:* Adaptable y mantiene la competitividad.
- *Cumplimiento Normativo:* Ayuda a cumplir regulaciones y estándares.
- *Visión Holística:* Proporciona una visión completa de la empresa.
- *Flexibilidad:* Adaptable a diferentes tipos de empresas.

**Ejemplos de ERP Conocidos:**

1. *SAP ERP:* Ampliamente utilizado a nivel mundial.
2. *Oracle ERP Cloud:* Soluciones en la nube para diversos sectores.
3. *Microsoft Dynamics 365:* Integración estrecha con herramientas de Microsoft.
4. *NetSuite:* Gestión empresarial en la nube, adquirido por Oracle.
5. *Infor ERP:* Soluciones específicas para diferentes sectores.
6. *Epicor ERP:* Enfocado en empresas de fabricación y distribución.
7. *Odoo:* ERP de código abierto con amplias aplicaciones empresariales.
8. *Sage X3:* Orientado a medianas y grandes empresas.
9. *IFS Applications:* Especializado en gestión de activos y fabricación.
10. *Acumatica:* ERP en la nube para finanzas, distribución y más.

## CRM (Customer Relationship Management)
**Características del CRM:**
1. *Gestión de Contactos y Clientes:* Centraliza información.
2. *Automatización de Ventas:* Optimiza procesos de venta.
3. *Gestión de Campañas de Marketing:* Planificación y seguimiento.
4. *Servicio al Cliente:* Atención eficiente y seguimiento.
5. *Análisis y Reportes:* Herramientas de análisis de datos.
6. *Integración con Plataformas:* Evita duplicación de datos.
7. *Acceso Móvil:* Información disponible en dispositivos móviles.
8. *Seguridad de Datos:* Medidas para proteger la información.

**Beneficios del CRM:**
1. *Mejora Relaciones con Clientes:* Comunicación personalizada.
2. *Aumento de Ventas:* Optimización del proceso de ventas.
3. *Eficiencia Operativa:* Automatización de tareas manuales.
4. *Mejora Retención de Clientes:* Seguimiento efectivo.
5. *Análisis Estratégico:* Toma de decisiones basada en datos.
6. *Eficiencia en Marketing:* Segmentación precisa.
7. *Adaptabilidad a Cambios:* Ajustes rápidos en estrategias.
8. *Acceso a Información en Tiempo Real:* Toma de decisiones más rápida.

9. **Ejemplos de CRM Conocidos:**

1. *Salesforce:* Ampliamente utilizado y versátil.
2. *HubSpot CRM:* Enfoque en inbound marketing y ventas.
3. *Microsoft Dynamics 365 CRM:* Integración con herramientas Microsoft.
4. *Zoho CRM:* Ofrece soluciones integrales para pequeñas y grandes empresas.
5. *Oracle CX Cloud:* Suite completa para experiencia del cliente.
6. *Pipedrive:* Especializado en gestión y automatización de ventas.
7. *SugarCRM:* Enfoque en flexibilidad y personalización.
8. *Freshworks CRM:* Soluciones escalables para diferentes empresas.
9. *Insightly:* Diseñado para pequeñas y medianas empresas.
10. *Zendesk Sell:* Integración con soporte al cliente y ventas.

## Business Intelligence (BI):
- *Definición:* Conjunto de procesos, tecnologías y herramientas que ayudan a convertir datos en información significativa para la toma de decisiones.

**ETL (Extract, Transform, Load):**
- Proceso de mover datos desde diversas fuentes, transformarlos para cumplir con requisitos empresariales y cargarlos en un almacén de datos.

**Data Warehouse:**
- Almacén centralizado de datos empresariales que facilita el análisis y la generación de informes.

**OLAP (Online Analytical Processing):**
- Procesamiento analítico en línea que permite la exploración multidimensional de datos para análisis avanzado.

**Data Mining:**
- Proceso de descubrimiento de patrones y relaciones significativas en grandes conjuntos de datos.

**Dashboard:**
- Herramienta visual que proporciona una representación gráfica de datos clave para facilitar la toma de decisiones.



