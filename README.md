# proyecto.23
Sistema de Historia Clínica y Evolución de Pacientes

Descripción General
Este proyecto es una aplicación de consola en Java que permite *registrar, consultar y administrar la información médica de pacientes*, incluyendo su historia clínica, evoluciones médicas, citas y medicamentos prescritos.

El sistema está diseñado como un ejercicio completo de Programación Orientada a Objetos (POO), integrando todos los conceptos fundamentales: encapsulamiento, herencia, polimorfismo, relaciones entre clases, manejo de excepciones y persistencia de datos.

Objetivos del Proyecto
- Aplicar los principios de la POO en un caso real.
- Implementar clases, objetos, atributos y métodos correctamente.
- Utilizar herencia, polimorfismo y encapsulamiento*}.
- Representar relaciones entre clases (asociación, agregación y composición).
- Implementar manejo de colecciones (ArrayList).
- Incluir gestión de excepciones y lectura/escritura de archivos.
- Crear un *menú interactivo por consola* para el usuario.

Conceptos POO Aplicados

Concepto | Ejemplo en el proyecto 

Encapsulamiento | Uso de atributos private y métodos get/set en todas las clases. 
Herencia | Medico y Paciente heredan de la clase abstracta Persona. 
Polimorfismo (Sobrescritura) | mostrarInfo() es sobreescrito en Medico y Paciente. 
Polimorfismo (Sobrecarga) | Métodos sobrecargados en la clase ArchivoManager. 
Composición | HistoriaClinica contiene una lista de EvolucionMedica. 
Agregación | EvolucionMedica agrega varios Medicamento. 
Asociación | CitaMedica se asocia a un Medico y un Paciente. 
Abstracción | Clase Persona y Interfaz Registrable. 

Clases Principales

Persona (abstracta) → Superclase de Medico y Paciente.  
Medico → Contiene especialidad, teléfono e ID.  
Paciente → Posee dirección, teléfono e historia clínica.  
HistoriaClinica → Contiene los antecedentes y evoluciones médicas.  
EvolucionMedica → Registra diagnóstico, tratamiento, observaciones y medicamentos.  
Medicamento → Representa el nombre, dosis y frecuencia del tratamiento.  
CitaMedica → Gestiona fecha, hora, motivo, médico y paciente.  
SistemaClinico → Clase principal que contiene los menús y listas de entidades.  
Registrable (Interfaz) → Define métodos para guardar y cargar datos.

Requerimientos Funcionales

1. Registro de pacientes y médicos: 
   - El sistema debe permitir ingresar los datos de nuevos pacientes y médicos por consola.
   - Los datos deben incluir nombre, edad, documento y otros atributos definidos.

2. Gestión de historias clínicas: 
   - Cada paciente debe tener una o varias historias clínicas.
   - Cada historia debe contener una lista de consultas médicas asociadas.

3. Registro de consultas: 
   - El médico podrá registrar consultas con información sobre fecha, motivo, diagnóstico y tratamiento.

4. Búsqueda de pacientes:
   - El sistema permitirá buscar pacientes por su número de documento.

5. Visualización de historial clínico:  
   - El usuario podrá consultar todas las historias y consultas asociadas a un paciente.

6. Persistencia de datos:  
   - La información de pacientes, médicos e historias clínicas debe guardarse y cargarse.

7. Interfaz por consola:  
   - El sistema mostrará un menú para navegar entre las opciones disponibles.
