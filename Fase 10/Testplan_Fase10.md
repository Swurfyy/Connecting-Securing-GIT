Fase 10:
Testplan:
- show ip interface brief
- show ip route
- show interfaces description
Verwacht resultaat:
Alle interfaces die aangemaakt zijn staan op "up/up"
Stap 2: Routing Verificatie
- show ip route
- show ip route bgp
- show ip route ospf
Verwacht resultaat:
Alle routes zijn zichtbaar in de routing table. BGP routes zijn aanwezig voor externe netwerken.
Stap 3: BGP Neighbor Verificatie
- show ip bgp summar
- show ip bgp neighbors
Verwacht resultaat:
Alle BGP neighbors tonen status "Established" & werken.
Stap 4: Connectiviteit Tests
Pingen tussen devices:
- Router NY -> Router BRU
- Router BRU -> Router NY
- Router NY -> R_Provider
- Router BRU -> R_Provider
Verwacht resultaat:
De pings zijn gelukt.
Stap 5: NAT/PAT
Commando’s op beide FW_NY & FW_BRU doen:
- show ip nat translations
- show ip nat statistics
- show ip access-list NAT_INTERNAL
Verwacht resultaat:
NAT access-list is correct geconfigureerd.
Fase 10:
Stap 6: Redundancy
Commando's:
- show ip bgp summary
- show ip interface brief
Verwacht resultaat:
Alle gegevens kloppen bij de show commando’s.
Stap 7: DHCP Configuratie
FW_NY:
- show ip dhcp pool
- show ip dhcp binding
- show running-config
Verwacht resultaat:
Configuratie klopt & DHCP is actief.