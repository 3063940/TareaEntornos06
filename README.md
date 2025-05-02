# Diseño estructural orientado a objetos a partir de un enunciado funcional

En el módulo de Programación se ha planteado una aplicación que permite gestionar distintos tipos de vehículos (coches, motos, camiones), con diferentes atributos y funcionalidades.

Se definen estructuras con **herencia**, **composición** e **interfaces**. Debes analizar y modelar un sistema completo basado en:

## Requisitos de modelado

- **Clase base abstracta:** `Vehículo`, con atributos comunes:
    - `matrícula: String`
    - `marca: String`
    - `modelo: String`
    - `kilometraje: double`
    - `precio: double`
    - Otros atributos necesarios

- **Subclases concretas:**
    - `Coche`
    - `Moto`
    - `Camión`

- **Subtipos específicos:**
    - `Coche`: `Sedán`, `SUV`, `Deportivo`
    - `Moto`: `Scooter`, `Deportiva`

- **Clase `Persona`:**
    - `nombre: String`
    - `apellidos: String`
    - `dni: String` (con validación)
    - `añoNacimiento: int`
    - `fechaCaducidadCarnet: LocalDate`

- **Relación de composición:**
    - Un `Vehículo` tiene (opcionalmente) un `propietario` de tipo `Persona`.

- **Interfaz `Valorable`:**
    - Implementada por los vehículos
    - Método para calcular la depreciación según el tipo de vehículo

- **Método de cálculo de riesgo:**
    - Determina el nivel de riesgo del conductor
    - Se basa en el tipo de vehículo y su experiencia

- **Tipos enumerados y reglas de negocio:**
    - Definidos en el documento adjunto
    - Deben reflejarse en el diseño

