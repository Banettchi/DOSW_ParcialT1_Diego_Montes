# DOSW_ParcialT1_Diego_Montes

## Realice el diagrama de contexto con las generalidades
<img width="385" height="241" alt="image" src="https://github.com/user-attachments/assets/2b964606-2369-42be-aeda-1ec96bb39af2" />

## Identifique 2 patrones de diseño que puedan aplicarse al caso de estudio,
## Primer patron
a. Abstract Factory

b. Tipo de patrón: Creacional

c. Ya que se van a manejar reservas en todas lo que varia es el tipo quien lo puede reservar o el tiempo asi que se pueden clasificar por interfaces para cada tipo de reserva ya sea sala, salon, oficina o equipo donde la clase abstracta puede ser una clase recurso para gestionar y crear las solicitudes para caada uno de los tipos 

## Segundo patron
a. Chain of Responsibility

b. Tipo de patrón: Comportamiento

c. Se puede manejar chain of responsability para el manejo de las solicitudes de reserva y verificar si el salon tiene la capacidad oo si esta disponible a la fecha y hora que se solicita y como no se debe verificar todo en una misma clase para no incumplir algunas practicas como el single responsability se puede usar este patron que verifique o si no pregunte a otro generando asi la cadena del factory method

## Identifique 5 requerimientos del sistema
### Funcionales (3)
Inicio de sesion 

Saber cual es el tiempo solicitado

Saber el numero de puestos

### No funcionales (2)

Tipologia visible y legible

Mantener colores alusivos al programa de Ingenieria de sistemas


# 📄 Requerimientos del Sistema

## 1. Lista general de requerimientos

El sistema de  Silabinfo tiene los siguientes requerimientos

### 1.1 Saber cual es el tiempo solicitado

El sistema de  Silabinfo debe tener la capacidad de:

1. Id de el lugar solicitado
2. Dia o fecha de la reserva
3. Hora inicio y hora final de la actual reserva
4. Hora final de la ultima reserva del lugar en esa fecha
5. Ocupacion del lugar

### 1.2 Saber el numero de puestos requeridos

El sistema de  Silabinfo debe tener:

1. Id de el lugar solicitado
2. Capacidad del lugar
3. Cantidad de usuarios que van a ingresar


## 2. Diagramas de caso de uso

### 2.1 Saber cual es el tiempo solicitado

| Campo | Descripción                                                                                                                                                                                                                                                                                                                           |
|------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID** | RF-01                                                                                                                                                                                                                                                                                                                                 |
| **Nombre del requerimiento** | Consultar el tiempo solicitado                                                                                                                                                                                                                                                                                                        |
| **Descripción** | *El sistema debe ser optimo al momento de la verificacion detiempos para no generar mas de una reserva en una misma fecha ademas de ser capaz de aceptar o rechazar si incumple alguna regla*                                                                                                                                         |
| **Precondiciones** | *Para que el sistema cumpla con este requerimiento, Silabinfo debe tener previamente el id del lugar que se solicito ademas de manejar la fecha de la reserva con la hora de inicio y saber cual es la ultima reserva que se realizo para ese dia para asi saber si se puede aceptar o rechazar ademas de saber si esta ocupada o no* |
| **Actor** | *Usuario*                                                                                                                                                                                                                                                                                                                             |
| **Flujo principal** | 1. El usuario informa cuanto tiempo planea ocupar el sitio de estudio<br>2. El sistema analiza si la fecha es una fecha optima y no una fecha expirada <br>3. El sistema verifica la disposicion del lugar si esta ocupado o no <br>4. El sistema acepta o rechaza la solicitud                                                       |
| **Diagrama de caso de uso** | * <img width="215" height="218" alt="image" src="https://github.com/user-attachments/assets/cc609044-e4b4-4531-b719-63e2b909cc26" /> *                                                                                                                                                                                                                                                                                                             |
| **Poscondiciones** | *Se espera como resultado saber cual es el tiempo que se va a usar la sala y su disposicion*                                                                                                                                                                                                                                          |

### 2.2 Saber el numero de puestos requeridos

| Campo | Descripción                                                                                                                                                                                                                                                                                                                                                       |
|------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID** | RF-02                                                                                                                                                                                                                                                                                                                                                             |
| **Nombre del requerimiento** | Consultar el numero de puestos                                                                                                                                                                                                                                                                                                                                    |
| **Descripción** | *El sistema debe tener la capacidad de mostrar los puestos que tiene a disposicion un sitio de estudio para que el usuario sea capaz de decidir si le sirve y si puede ocupar el lugar de una manera optima*                                                                                                                                                      |
| **Precondiciones** | *Para que el sistema cumpla con este requerimiento, Silabinfo debe tener previamente el id del lugar solicitado su capacidad y la cantidad de usuarios que la piensan ocupar para saber si es optimo o no*                                                                                                                                                        |
| **Actor** | *Usuario*                                                                                                                                                                                                                                                                                                                                                         |
| **Flujo principal** | 1. El usuario solicita una sala de una cantidad de puestos <br>2. El sistema verifica que la sala este ocupada o disponible <br>3. El sistema  verifica las horas que el usuario piensa usar la sala <br>4. El sistema verifica el tamaño de el lugar solicitado y compara con los puestos solicitados <br>5. El sistema rechaza o acepta la solicitud de reserva |
| **Diagrama de caso de uso** | * <img width="223" height="187" alt="image" src="https://github.com/user-attachments/assets/3cccafab-d446-4f9f-812d-8c98e74b1d1f" />*                                                                                                                                                                                                                                                                                                                                             |
| **Poscondiciones** | *La cantidad de puestos que se usan o que estan disponibles en un lugar de estudios para verificar si el lugar es util para el usuario o no*                                                                                                                                                                                                                      |


## Requerimiento asociado

### Epica
Al ser un gran bloque de trabajo la epica es el caso de la manera mas grande es decir la cantidad de tiempo que se piensa utilizar el lugar de estudio
### Historia de usuario
Establecer un sitio web que permita seleccionar la fecha y las horas ademas del lugar que desea solicitar y si tiene la autorizacion de hacerlo

### Tareas
requisitos funcionales desde la perspectiva del usuario

1 Poder colocar una hora inicial de tiempo

2 Poder colocar la cantidad de tiempo que piensa usar el lugar

3 Poder colocar una fecha del dia que pienso usar el lugar

4 Realizar una consulta de si se puede el lugar que quiero

5 enviar la solicitud

## Diagrama de clases

<img width="418" height="257" alt="image" src="https://github.com/user-attachments/assets/ad6eb827-e879-451f-a39e-a18b5b3d8a14" />
