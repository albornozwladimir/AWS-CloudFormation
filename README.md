# AWS-CloudFormation
Infrastructura como código para modelar y aprovisionar ciertos recursos de AWS

## Cloudformation - (https://aws.amazon.com/cloudformation/)
Las siguientes plantillas permiten crear recursos en AWS tanto por el cliente AWS como directamente en la consola web, previa configuración

### Función Lambda
Sin preocuparnos de la infraestructura permite ejecutar funciones.

1. Esta solución permite crear mediante CloudFormation una función Lambda mediante una URI de imagen Docker(alojada previamente en AWS ECR)
2. Asociada a la función Lambda existe una regla programada que permite invocar la misma mediante una expresión CRON (AWS::Events)
3. Se genera un permiso asociada a la función Lambda que permite su ejecución
