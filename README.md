# Spring IoC para .NET

➡️ Curso relacionado: **[Spring IoC para .NET](https://stahe.github.io/ales-springioc-dotnet-avril-2005/)**

Este documento presenta los principios de la **inversión de control (IoC)** y su implementación en el ecosistema **.NET** mediante el marco **Spring.NET**, una adaptación del marco **Spring** diseñado originalmente para Java. 

El objetivo es mostrar cómo se puede mejorar el diseño de las aplicaciones al **desacoplar los componentes** y dejar que un contenedor de configuración se encargue de su ensamblaje.

---

# Objetivos de este documento

Este tutorial tiene los siguientes objetivos:

- descubrir las posibilidades de **configuración e integración del marco Spring** en una aplicación .NET  
- comprender el concepto de **Inversión de control (IoC)**  
- aprender cómo se puede utilizar la **inyección de dependencias (Dependency Injection)** para desacoplar componentes  
- aplicar estos conceptos en **ejemplos concretos en VB.NET** 

---

# Antecedentes

Las ideas que se presentan en este documento están fuertemente inspiradas en el libro de **Rod Johnson**:

**J2EE Development without EJB (Wrox, 2004)**

Este libro sentó las bases de la filosofía de Spring: crear aplicaciones más sencillas, más modulares y más fáciles de probar, evitando las fuertes dependencias de los marcos tradicionales.

Ya existe un documento similar para **Spring / Java**.  
Este tutorial retoma los mismos conceptos y **los adapta a la plataforma .NET**. 

---

# Spring.NET

Al momento de escribir este documento:

- **Spring.NET** está disponible en la versión **0.6 RC3 (abril de 2005)**  
- solo se han implementado ciertas funcionalidades del Spring Java original  
- sin embargo, las funcionalidades esenciales sí están disponibles:

- **Inversión de control (IoC)**
- **Programación orientada a aspectos (AOP)**

Este tutorial se enfoca principalmente en **IoC**, que constituye el núcleo de la filosofía de Spring. 

---

# Principio: Inversión de control (IoC)

En una arquitectura clásica:

- un objeto crea sus propias dependencias;
- el objeto controla directamente a los objetos que necesita

Con **IoC**:

- las dependencias **son inyectadas por un contenedor**
- los componentes están **débilmente acoplados**
- la configuración se **externaliza**

Esto garantiza:

- una **mejor mantenibilidad**
- una **mayor capacidad de prueba**
- una **arquitectura más flexible**

---

# Ejemplos prácticos

La sección práctica del documento contiene varios ejemplos que ilustran lo siguiente:

- la configuración de los componentes de Spring.NET
- la inyección de dependencias
- la creación de objetos de negocio desacoplados

Los ejemplos están escritos en **VB.NET**.

Las pruebas utilizan el marco **NUnit**, el equivalente en .NET del marco **JUnit** que se utiliza en el ecosistema Java. 

---

# Requisitos

Para poder seguir los ejemplos:

- Entorno **.NET**
- **Spring.NET**
- **NUnit** para ejecutar pruebas unitarias

En los anexos del documento se explica:

- dónde se pueden descargar estas herramientas
- cómo se deben instalar

---

# Filosofía de Spring

La ventaja más importante de Spring no radica solo en los mecanismos técnicos, sino sobre todo en su **filosofía de diseño**:

- separación de responsabilidades  
- acoplamiento débil entre componentes  
- configuración externa de las dependencias  
- arquitectura orientada a pruebas

Estos principios permiten diseñar aplicaciones **más sencillas, más modulares y más robustas**.

