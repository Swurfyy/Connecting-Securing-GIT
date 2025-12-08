
Testplan:

- show ip interface brief
- show interfaces description
Verwacht resultaat:
Alle interfaces die aangemaakt zijn staan op "up/up"

Stap 2: ACL Verificatie
Commando's op CSW1 & CSW2:
- show ip access-lists
- show ip access-group
Verwacht resultaat:
Alle ACL's zijn correct geconfigureerd en toegepast.
Stap 3: ACL Functionaliteit
Pingen tussen VLANs:
- VLAN 10 -> VLAN 20 (moet geblokkeerd worden)
- VLAN 10 -> DHCP server 10.4.6.10 (moet werken)
- VLAN 20 -> DHCP server 10.4.6.10 (moet werken)
Verwacht resultaat:
VLAN 10 en VLAN 20 kunnen niet met elkaar communiceren. DHCP verkeer werkt.
Stap 4: Port Security
Commando's op L2-S1 & L2-S2:
- show port-security
- show port-security address
Verwacht resultaat:
Port security is actief op access poorten.
Stap 5: DHCP Snooping
Commando's op L2-S1 & L2-S2:
- show ip dhcp snooping
- show ip dhcp snooping binding
Verwacht resultaat:
DHCP snooping is actief. Trunk poorten zijn trusted.
Stap 6: STP Protection
- show spanning-tree summary
- show spanning-tree guard
Verwacht resultaat:
BPDU Guard en Root Guard zijn correct geconfigureerd.
Stap 7: Connectiviteit Test
Pingen:
- VLAN 10 -> SERVERS VLAN
- VLAN 20 -> SERVERS VLAN
- VLAN 10 -> MGMT VLAN
Verwacht resultaat:
De pings zijn gelukt.

