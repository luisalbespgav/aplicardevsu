Diseño de Soluciones utilizando el Modelo C4

El modelo C4 es un enfoque visual para documentar y comunicar la arquitectura de software de forma clara y estructurada. 
Un buen diagrama de arquitectura de software facilita la comunicación a los equipos de desarrollo y producto, la idea principal es que los diagramas puedan ser entendidos e interpretados por equipos técnicos y no técnicos.

Cuenta con cuatro niveles de abstracción, de ahí su nombre:
	Nivel 1: Diagrama de Contexto. 
	Nivel 2: Diagrama de Contenedores
	Nivel 3: Diagrama de Componentes
	Nivel 4: Diagrama de Código (opcional)
Estos permiten mejorar la documentación de proyectos completos a fin de que la audiencia pueda comprender en que consiste, como esta conformado y como se interrelaciona con otros sistemas o servicios.


 
Objetivo:
Diseñar un Sistema de Banca por internet, que permita:
	Crear clientes
	Consultar Información de los clientes
	Realizar transferencias bancarias e interbancarias
	Realizar pagos con debido a cuenta
	Configuración de cupos para transferencias
	Consulta de movimientos Histórico


Consideraciones:
Realizaremos un Análisis y Diseño de un Sistema de Banca Electrónica Web de una entidad BP, considerando los siguientes aspectos:
1.	Solo puede ser accedido por clientes del banco
2.	Cuenta con un esquema de autenticación y autorización (Azure Entra ID)
3.	Cuenta con un modelo de factor de autenticación mediante OTP (Contraseña de un Solo Uso) que se enviará al teléfono celular del usuario como SMS o Push Notification, o email
4.	La OTP tiene un tiempo de vigencia de 3 minutos, caso contrario caduca y deniega el acceso
5.	Valida que el usuario se encuentre activo en el banco
6.	El sistema permite consultar Posición Consolidada y Estados de Cuenta considerando el histórico de movimientos de los clientes
7.	Cuenta con un base de datos de Core Bancario y una base de datos de Master Data Management (MDM) con información adicional y detallada del cliente
8.	Permite consultar y actualizar cupos para transacciones y pagos de las cuentas de clientes
9.	Permite realizar transferencias bancarias e interbancarias
10.	Permite realizar pagos de servicios con debido a cuenta
11.	Envía un mensaje al usuario (cliente) como SMS o Push Notification, o email, cuando se ha realizado una transacción bancaria
12.	Permite guardar logs de auditoría del sistema y transaccionales en un repositorio como Elasticsearch
13.	Debe manejar esquemas de anonimización y cifrado para datos sensibles, especialmente los del cliente
14.	Debe permitir el registro y uso de acceso biométrico
