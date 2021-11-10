##### 4 - Cines y Películas
- CINE(__Nombre__,calle,nTelefono)
- TARIFAS(__Dia__,__Precio__,Nombre(FK=>CINE))
- PASA(__Nombre(FK=>CINE)__,__Titulo(FK=>PELICULA)__,hora)
- PELICULA(__Titulo__,director,genero,clasificacion)
- PROTAGONISTA(__Nombre__,Titulo(FK=>PELICULA))

##### 5 - Proyectos de Investigación
- PROYECTO(__Nombre__,fechaInicio,tipo)
- NUEVO-P(__Nombre=>PROYECTO__,presupuesto)
- REVISION-P(__Nombre=>PROYECTO__,motivo)
- INVESTIGADOR(__DNI__,nombre,apellidos,direccion,telefono,localidad,__Nombre=>PROYECTO__)
- INVESTIGADOR-SUPERVISOR(__DNI=>INVESTIGADOR__,__DNI=>INVESTIGADOR__)
- REALIZA-CONFERENCIA(__DNI=>INVESTIGADOR__,__Nombre=>CONFERENCIA__)
- CONFERENCIA(__Nombre__,fechaHoraInicio,lugar,nHoras)

##### 6 - Universidad
- PERSONA(__pID__,nombre,dir,tfno,emai,tipo)
- PERSONA-PROFESOR(__pID=>PERSONA__,ded)
- PERSONA-ALUMNO(__pID=>PERSONA__,exp,titulacion,nombreC=>CENTRO)
- PERSONA-PERSONAL(__pID=>PERSONA__,unidad,cat)
- PROFESOR-IMPARTE(__nombreC=>CENTRO__,__pID=>PERSONA-PROFESOR__)
- CENTRO(__nombreC__)

##### 7 - Agencia de alquileres
- PROPIETARIO(__DNI__,nombre,tlfno)
- CLIENTE(__DNI__,nombre,tlfno)
- TEMPORADA(__Quincena__,__Mes__,__Anno__)
- APARTAMENTO(__Cod_apart__,DNI=>PROPIETARIO,direccion,tipo,num_hab,m2,p_linea_de_playa)
- COSTE-AP-TEMP(__Cod_apart=>APARTAMENTO__,__Quincena=>TEMPORADA__,__Mes=>TEMPORADA__,__Anno=>TEMPORADA__)
- ALQUILER()
