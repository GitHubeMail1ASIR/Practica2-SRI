# Practica2-SRI

## Descripción 📋

Vamos a continuar trabajando en el escenario que desarrollamos en la Práctica: Creación y configuración de un escenario router-nat.

Queremos crear un playbook de ansible que instale un servidor DHCP en la máquina router para que configure de forma automática las máquinas que se conectan en la red interna. Tenemos que tener en cuenta lo siguiente:

1. La máquina cliente de la práctica anterior, que tiene instalado el servidor web, debe tener la misma IP que la que le asignaste estáticamente (10.0.0.2), por lo tanto haremos una reserva para que tenga la misma IP.

2. Al añadir una nueva máquina a la red local (recuerda que no se le instalará el servidor web) se configurará de forma dinámica.

3. Crea un nuevo rol en el playbook de ansible llamado dhcp que configure el servidor DHCP de forma correcta. Quizás sea necesario modificar el comportamiento de algún rol de la práctica anterior.

4. Todos los parámetros que reparta el servidor DHCP, así como cualquier otro dato, por ejemplo la dirección MAC del cliente se guardarán en variables.

5. Añade una nueva máquina al escenario conectada a la red interna muy aislada (10.0.0.0/24). Vuelve a ejecutar el playbook y comprueba que todo funciona de forma correcta.

## Entrega 📋

1. Entrega la URL del repositorio GitHub donde has alojado todos los ficheros.
2. Entrega el fichero de configuración del servidor DHCP después de ejecutar el playbook de ansible.
3. Entrega el fichero de configuración de red del cliente (para comprobar que toma direccionamiento dinámico) y que ha tomado la dirección reservada en el servidor DHCP.
4. Entrega el fichero de configuración de red de la otra máquina cliente, la dirección que ha tomado y el fichero de concesiones del servidor donde se demuestra que se ha repartido.
5. Comprueba que la nueva máquina cliente no tiene el servidor apache2 instalado, y una captura de pantalla comprobando que sigue siendo accesible el servidor web de cliente.

🔗 **Información de la tarea extraída de: https://fp.josedomingo.org/sri2223/2_dhcp/practica.html**

## Autor ✒️

* **Juan Jesús A. S.** - *Gonzalo Nazareno*