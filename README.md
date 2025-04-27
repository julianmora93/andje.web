# AndjeWeb

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 15.2.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

## NOTAS

Dialog Victimas: 
 => Victima Directa es si/no
 => Sexo: Listado proviene dde un servicio (pendiente Gian)
 => Cada peticionario debe relacionar la victima de su peticion pero no siempre va a tener victimas
    ==> Ej: 
        - Peticionario: Julian
        - Victima: Julian
        - Victima Directa: Si
        ----
        - Peticionario: Julian
        - Victima: Yesica
        - Victima Directa: Si
 => Se debe incluir el servicio de parentezcos (pendiente Gian)



Dialog Conflicto armado:
 => Si el toggle esta en true habilita el listado, si esta el false l.o deshabilita y no agrega ningun macrocaso









Nombre de Peticion: 
    Caso Julian Mora V001

Número de caso:
    P-20587J

Número petición:
    20101203D50-1

Etapa Procesal:
    1

Instancia:
    1

Expediente:
    20241545AVC660








Inputs: 
 > Fecha => Datepicker
 > Entidad => Search(WS: Activity)
 > Actividad => Search(Dependiente de actividad seleccionada - WWS: EntityOfActivity)
 > Soporte => InputText
 > Accion pendiente => Search(WS: PendientePorGIAN)
 > Vencimiento inicial => Datepicker *no es obligatorio
 > Vencimiento maximo => Datepicker *no es obligatorio
 - pude que no tenga ninguna de las 2 fechas
 - puede que tenga la primer fecha
 - puede que tenga la segunda fecha pero solo si la primera existe




REPORTES GRAFICOS
================================================
PIE [Portafolio SIDH]
https://www.highcharts.com/demo/pie-basic/grid-light
------------------------------------------------
Corte: 31/03/2023
------------------------------------------------
ETAPA						NUMERO DE CASOS
------------------------------------------------
Admisibilidad				495
Fondo 						300
Admisibilidad y Fondo		73
Articulo 50					15
Solución amistosa			26
Casos contenciosos (Corte)	7
------------------------------------------------
Total: 916
------------------------------------------------




================================================
BAR [Vencimiento por mes de las etapas procesales]
https://www.highcharts.com/demo/bar-basic/grid-light
------------------------------------------------
Año: 2023
------------------------------------------------
Mes: Abril
Admisibilidad: 25
Fondo: 2
Admisibilidad y fondo: 0
--
Mes: Mayo
Admisibilidad: 9
Fondo: 12
Admisibilidad y fondo: 3
--
Mes: Junio
Admisibilidad: 12
Fondo: 2
Admisibilidad y fondo: 0
--
Mes: Julio
Admisibilidad: 10
Fondo: 5
Admisibilidad y fondo: 0
------------------------------------------------




================================================
GAUGE [Porcentaje cumplimiento indicadores]
https://www.highcharts.com/demo/gauge-activity/grid-light
------------------------------------------------
Indicador Mensual: Corte a Marzo
--
Adminisibilidad: 20 vencimiento -> presentaron 18 [95%]
Fondo: 15 vencimiento -> presentaron 10 [90%]
Admisibilidad y fondo: 5 vencimientos -> presentaron 5 [100%]
------------------------------------------------



















----------------------------------------------------------------------
------------------------------ NACIONAL ------------------------------
----------------------------------------------------------------------
-- LegisOffice --
-----------------
Menu: 
--
- Mi Oficina
    - Estado de mis casos
    - Gestion de mis actividades
    - Actuaciones Judiciales
    - Reportes mas usados
    - Casos recientes
    - Documentos recientes
- Mis Casos
- Mis Actividades
- Actuaciones Judiciales
- Anotaciones
--
- Reportes
- Reportes +
- Directorio
- Documentos
- Minutas
- Papelera
--
- Administrador

---------------------
-- Campos del Caso --
---------------------
OK - Nombre del caso => string
OK - Numero eKOGUI => string
OK - Estado del proceso => combo
OK - Año terminado => date
OK - Instancia => combo
OK - Numero radicado => string
OK - Despacho => string
OK - Demandante principal => string
OK - Tipo de caso => combo
OK - Ultima actuacion judicial => string
OK - Valor economico indexado  => string
OK - Erogacion economica => string
OK - Tipo de providencia => combo
OK - Otra providencia => string
OK - Sentido del fallo en 1 o unica instancia => combo
- Fecha fallo 1 o unica instancia => date
- Fecha notificacion fallo 1 instancia => date
- Sentido en fallo en 2 instancia => combo
- Fecha fallo 2 instancia => date
- Fecha notificacion dallo 2 instancia => date
- La providencia esta ejecutoriada => combo
- Monto condena => string
- Descripcion del logro => textarea
- Aprobacion Director DDJN => combo
- Caso Acumulado => combo
- #CUP al que acumula => string
- Expediente ORFEO => string
- Fecha PRE-IRUC => date
- Fecha IRUC => date
- Coordinador => combo
- Hechos => textarea
- Proceso Prioritario => combo
- Intervencion Masiva => combo
- Area de practiva => combo
- Codigo PAI => combo






actual.state.entity
control.medium.entity
defendant.entity
dispatch.entity
judge.oroffice.magistrate.entity
jurisdiction.entity
management.entity
management.objetive.entity
manager.entity
municipality.entity
national.instance.entity
national.procedural.stage.entity
practice.area.entity
principal.agent.entity
substitute.agent.entity
who.project.entity