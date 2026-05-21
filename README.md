# Portal de Orientación Laboral e Información de Derechos 

Este proyecto consiste en una aplicación web dinámica orientada a la divulgación de derechos, conceptos básicos de la relación laboral y la promoción de un entorno de trabajo digno y con respeto (inspirado en iniciativas de apoyo social como Médicos del Mundo). El sistema está programado en **PHP estructurado bajo Programación Orientada a Objetos (POO)** y **PDO**, garantizando modularidad, escalabilidad y un panel administrativo robusto.

## Características Principales 

* **Gestión de Contenidos Dinámicos (Bloques):** Arquitectura flexible que permite renderizar tarjetas informativas en cuadricula (*grids*) según categorías y subcategorías, extrayendo los textos directamente desde la base de datos de manera limpia.
* **Módulo de Preguntas Frecuentes (FAQ) Jerárquico:** Soporte para un sistema de FAQ multinivel mediante relaciones madre-hija en la base de datos, facilitando una navegación fluida por temáticas legales y de soporte.
* **Secciones de Concienciación Social:** Vistas dedicadas y adaptadas (diseño limpio estilo informativo) para temas clave como conceptos contractuales, dignidad, protocolos contra el acoso en el trabajo y el derecho a la intimidad.
* **Panel de Administración Centralizado:** Control total para administradores que permite listar usuarios, dar de alta nuevas cuentas con asignación de roles, y realizar operaciones CRUD completas (crear, editar, eliminar) sobre las preguntas frecuentes y contenidos de los bloques.
* **Arquitectura de Software Limpia:** Separación de responsabilidades mediante clases independientes (`Bloque`, `Categoria`, `Faq`, `Usuaria`, `GestionAdmin`) y conexión centralizada mediante el objeto `Database`.

## Tecnologías Utilizadas 

* **Backend:** PHP 8.x con Programación Orientada a Objetos (POO) y abstracción de datos mediante **PDO (PHP Data Objects)**.
* **Base de Datos:** MySQL / MariaDB (`medimundohome`) con un esquema relacional para usuarios, categorías, bloques de contenido y FAQs.
* **Seguridad:** Consultas parametrizadas mediante Sentencias Preparadas en PDO (`prepare` y `bindParam`) para mitigar vulnerabilidades de inyección SQL (SQLi).
* **Frontend:** HTML5 semántico, CSS3 y Javascript personalizado con un sistema de diseño basado en componentes responsivos y paletas de colores accesibles.
