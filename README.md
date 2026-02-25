# DOSW_ParcialT1_Diego_Montes

## Identifique 2 patrones de diseño que puedan aplicarse al caso de estudio,
### especificando por cada uno:
#### a. Nombre del Patrón
#### b. Tipo de patrón (creacional, estructural o de comportamiento).
#### c. Justificación de la decisión.

## Primer patron
### a. Abstract Factory
### b. Tipo de patrón: Creacional
### c. Ya que se van a manejar reservas en todas lo que varia es el tipo quien lo puede reservar o el tiempo asi que se pueden clasificar por interfaces para cada tipo de reserva ya sea sala, salon, oficina o equipo donde la clase abstracta puede ser una clase recurso para gestionar y crear las solicitudes para caada uno de los tipos 

## Segundo patron
### a. Chain of Responsibility
### b. Tipo de patrón: Comportamiento
### c. Se puede manejar chain of responsability para el manejo de las solicitudes de reserva y verificar si el salon tiene la capacidad oo si esta disponible a la fecha y hora que se solicita y como no se debe verificar todo en una misma clase para no incumplir algunas practicas como el single responsability se puede usar este patron que verifique o si no pregunte a otro generando asi la cadena del factory method

