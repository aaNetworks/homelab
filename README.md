### Ariel Antigua Networks (aaNetworks)
### homelab infrastructura.

### Iniciemos con el hardware.

- networking:

    En esta sección tenemos varios routers y switches.

        WAN1 – este es el equipo que la mayoría tenemos en casa, es asignado por CLARO para los clientes con Fibra Óptica, mi velocidad de internet actual es 200Mbps/20Mbps.
        WAN2 – Internet de Orbit Cable, entregado vía Fibra Óptica. Solo tiene 4Mbps/2Mbps, lamentablemente esta detrás de CGNAT.
        firewall – Sophos XG 115 corriendo pfSense+ 22.05
        nixon – Mikrotik RB3011-RM – este equipo forma parte de una nube MPLS y es un router de borde.
        zapp – Mikrotik RB2011-RM – este es el route principal de la red.
        lrrr –   Mikrotik RB493AH – router para pruebas de PPPoE, MPLS y VPLS.
        brrr –  Mikrotik RB750Gr3 – router para pruebas de PPPoE, MPLS y VPLS.
        ndnd – Mikrotik RB2011L-RM – router para pruebas de PPPoE, MPLS y VPLS.
        elzar – Mikrotik RB2011-RM – router para pruebas de PPPoE, MPLS y VPLS.
        CORESW0 – Mikrotik CRS226-24G-2S+ – Switch principal de la red.
        Atlas1 – RIPE Atlas sensor (Probe #28779) – este equipo directamente no se controla, es parte del proyecto Atlas de RIPE NCC. (¡¡¡4 anos en funcionamiento !!!)
        Atlas2 – RIPE Atlas Sensor (Probe #51981) – este sensor reporta estadísticas usando el internet de CLARO.
        Atlas3 – RIPE Atlas Sensor (Probe #XXXXX ) – este sensor reporta estadísticas usando el internet de ORBIT.
        Ubiquiti UCK – Generación 1 cloud key.


- servers:

    Supermicro demacomisionado.

        Intel(R) Atom(TM) CPU D2500 @ 1.86GHz
        6GB de RAM
        SSD 60GB Sandisk
        2x 1Gb NIC
        node17 – Ubuntu Server 20.04 – Es un mini-pc Lenovo M700, temporalmente en un cluster de Kubernetes.


    store – unRAID 6 – almacenamiento centralizado para las necesidades de File Services. Además de storage con unRAID se tiene la facilidad de correr Docker/VM. Alguno de los contenedores corriendo aquí son Plex, Syncthing, Sonarr, Radarr y algún otro que olvide ahora mismo.

        Ahora es una VM en ESXi7.0 (esxi1)
        Supermicro X9SRL
        Intel Xeon E5-2680 v2
        96GB de RAM
        2x 2TB Hard disks
        2x 4TB Hard disks
        2x 3TB Hard disks
        1x Intel SSD PCIe 1.6 TB
        More SSDs for VMs….
        2x 1Gb NIC
        10Gb NIC – aún no se ha conectado, el CRS cuenta con dos puertos 10GB.
        Rosewill RSV-L4000 – 4U



![image](images/homelab_20231208.jpeg)