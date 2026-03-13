# Secure-Network-Architecture-GNS3
Diseño y despliegue de infraestructura de red segura: VPN Site-to-Site, túneles GRE sobre IPSec y enrutamiento dinámico OSPF en entornos Cisco.
Secure Site-to-Site VPN & OSPF Infrastructure

!Topoligia(Imagenes/topologia.JPG)

🌐 Resumen del Proyecto

Simulación de una red corporativa de alta disponibilidad utilizando GNS3. El proyecto demuestra la capacidad de interconectar oficinas geográficamente distantes de forma segura y automática.

🛡️ Características Técnicas

Seguridad (VPN): Implementación de Túneles IPSec con cifrado AES-256 y autenticación SHA para garantizar la integridad de los datos.

Encapsulación: Uso de GRE (Generic Routing Encapsulation) para el transporte de tráfico Multicast (necesario para el enrutamiento OSPF) sobre la VPN.

Enrutamiento: Configuración de OSPF v2 con ID de router único y optimización de áreas.

Servicios de Red: - NAT Overload (PAT): Traducción de direcciones privadas para acceso a internet.

DHCP Server: Asignación automática de IPs por VLAN.

ROAS (Router on a Stick): Gestión de tráfico Inter-VLAN.

📁 Estructura del Proyecto

/configs: Archivos de configuración (running-config) de los routers R2 y R3.

/topology: Diagrama de red y esquema de direccionamiento.

/docs: Informe técnico paso a paso en PDF.

🚀 Comprobación de Estado (Troubleshooting)

Se validó la infraestructura mediante:

show crypto isakmp sa: Verificación del túnel fase 1.

show ip ospf neighbor: Confirmación de adyacencias dinámicas.

ping: Pruebas de latencia y conectividad extremo a extremo.

Christian Alberto Quispe Alarcón Ingeniero de Ciberseguridad en formación | Analista SOC
