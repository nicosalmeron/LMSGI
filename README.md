# LMSGI
Cuaderno lenguaje de marcas. Nicolás Salmerón Salvador. CFGS 1ºASIR.
## Tabla de contenidos
* [Qué es un Lenguaje de marcas](https://github.com/nicosalmeron/LMSGI#qu%C3%A9-es-un-lenguaje-de-marcas)
* [Evolución de los Lenguaje de marcas](https://github.com/nicosalmeron/LMSGI#evoluci%C3%B3n-de-los-lenguaje-de-marcas)
* [Características de los lenguajes de marcas](https://github.com/nicosalmeron/LMSGI#caracter%C3%ADsticas-de-los-lenguajes-de-marcas)
* [Características y ejemplos de los siguientes lenguajes de marcas:](https://github.com/nicosalmeron/LMSGI#caracter%C3%ADsticas-y-ejemplos-de-los-siguientes-lenguajes-de-marcas)
* [XML: definición y características del metalenguaje](https://github.com/nicosalmeron/LMSGI#xml-definici%C3%B3n-y-caracter%C3%ADsticas-del-metalenguaje)

## Qué es un Lenguaje de marcas
Un lenguaje de marcas es un conjunto de instrucciones especiales que usamos para darle al ordenador, es información sobre cómo mostrar o estructurar texto y otros contenidos. Es como dar direcciones para que sepa cómo mostrar un documento. En lugar de usar palabras, usamos símbolos y etiquetas para definir cómo debe de verse todo.

## Evolución de los Lenguaje de marcas
- GML
  1. Es un lenguaje que se usa para mostrar información cartográfica en geografía, por ejemplo.
- SGML
  1. Es un lenguaje que sirve como base para hacer otros lenguajes de marcado, algunos ejemplos son HTML y XML

## Características de los lenguajes de marcas

Hay que recalcar que los lenguajes de marcas NO son lenguajes de programación, dicho esto estas son las caracteristicas de los lenguajes de marcas:

1. **Sintaxis Simple**: Utilizan etiquetas o marcadores para definir la estructura y el formato.
2. **Independencia del Formato**: Separan el contenido de la presentación.
3. **Legibilidad Humana y Máquina**: Son legibles tanto por humanos como por máquinas.
4. **Ampliamente Utilizados**: Se utilizan en tecnología de la información.

## Características y ejemplos de los siguientes lenguajes de marcas:
- XML : XML es muy extensible, esto significa que se pueden crear estructuras de datos personalizadas y poner etiquetas según nuestras necesidades, se usa en sitios web, bases de datos, etc...
  ```
  <pizzas>
    <link type="text/css" rel="stylesheet" id="dark-mode-custom-link"/>
    <link type="text/css" rel="stylesheet" id="dark-mode-general-link"/>
  <style lang="en" type="text/css" id="dark-mode-custom-style"/>
    <style lang="en" type="text/css" id="dark-mode-native-style"/>
    <style lang="en" type="text/css" id="dark-mode-native-sheet"/>
  <pizza nombre="Barbacoa" precio="8">
    <ingrediente nombre="Salsa Barbacoa"/>
    <ingrediente nombre="Mozzarella"/>
    <ingrediente nombre="Pollo"/>
    <ingrediente nombre="Bacon"/>
    <ingrediente nombre="Ternera"/>
  </pizza>
  <pizza nombre="Margarita" precio="6">
    <ingrediente nombre="Tomate"/>
    <ingrediente nombre="Jamón"/>
    <ingrediente nombre="Queso"/>
  </pizza>
  </pizzas>
  ```
- HTML : Es un lenguaje de marcado que permite insertar enlaces, multimedia, y estilos con CSS. Se usa para construir sitios web principalmente.
```
<html>
	<head>
		<title>Mi página de ejemplo</title>
	</head>
	<body>
	Aquí va el contenido
	</body>
</html>
```
- JSON : Este lenguaje de marcado sirve para intercambiar datos entre una aplicación y un servicio web. Es bastante entendible por los humanos y se caracteriza por tener una estructura jerarquica. Hace uso de una sintaxis "clave-valor".
```
{
  "nombre":"Jonh Doe",
  "profesion":"Programador",
  "edad":25,
  "lenguajes":["PHP","Javascript","Dart"],
  "disponibilidadParaViajar":true,
  "rangoProfesional": {
      "aniosDeExperiencia": 12,
      "nivel": "Senior"
  }
}
```
- YAML: Es otro lenguaje de marcado que se usa en archivos de configuración principalmente. Un ejemplo bastante conocido es el famoso "Netplan" que se presenta en la mayoría de distribuciones Linux derivadas de Debian.
```
network:
  version: 2
  renderer: NetworkManager
  ethernets:
   enp0s3:
    dhcp4: no
    addresses
    - 192.168.0.20/24
    gateway4: 192.168.0.1
    nameserver:
     addresses: [192.168.0.20]
```

## XML: definición y características del metalenguaje
- Prologo
  Es la parte del archivo XML en la cual se definen algunos parametros, como la versión o la codificación.
- Contenido
  Es el contenido del archivo XML, al principio se marca la etiqueta root y lo comprendido entre la etiqueta de apertura y cierre es el contenido.
- Atributo
  Son los valores que se usan para aportar información. Están dentro de las etiquetas.
- Ejemplos en XML
```
<?xml version="1.0" encoding="utf-8" standatone"no" ?>

    <root>
     <client dni "11111111H">
        <name> pepe </name>
        <lastname> perez </lastname>
     </client>

    <products>
        <product fechainicio="3-3-3" fechafin="4-4-4">
            <name> Producto 1 </name>
        </product>

        <product fechainicio="1-1-1" fechafin="7-7-7">
            <name> Producto 2 </name>
        </product>
    
    </products>
    </root>
```
