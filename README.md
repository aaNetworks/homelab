## This is Ariel Antigua Networks
## homelab infrastructure documentation.

### Let's start with hardware.

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