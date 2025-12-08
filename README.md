# Connecting-Securing-GIT
De GIT voor Connecting &amp; Securing Networking | Documentatie


# 1. Welke devices hebben welke functie? | Rechterzijde 
## Routers:
- De bovenste router:
  
- De middelste router:
  
- De onderste router

## Switches
### Layer 3:
- 1. De bovenste L3:
Dit is de CSW 1 Switch.

- 2. De onderste L2:
Dit is de CSW 2 Switch.

### Layer 2:
- 1. De bovenste L2:
Dit is L2-S1.

- 2. De onderste L2:
Dit is de L2-S2.

# Poorten per toestel:

## CSW1:
- Fa0/1 -> L2-S1 Fa0/1
- Fa0/3 -> L2-S2 Fa0/3
- Fa0/23 -> CSW2 Fa0/23
- Fa0/24 -> CSW2 Fa0/24
- Fa0/20 -> PaloAlto 0/3


## CSW2
- Fa0/1 -> L2-S1 Fa0/2
- Fa0/3 -> L2-S2 Fa0/4
- Fa0/23 -> CSW1 Fa0/23
- Fa0/24 -> CSW1 Fa0/24
- Fa0/20 -> PaloAlto 0/4

## L2-S1
- Fa0/1 -> CSW1 Fa0/1
- Fa0/2 -> CSW2 Fa0/1

## L2-S2
- Fa0/3 -> CSW1 Fa0/3
- Fa0/4 -> CSW2 Fa0/3
-

## Palo Alto Brussel
-
-
-

## Region Provider Router
-
-
-

# 2. Welke devices hebben welke functie? | Linkerzijde 

## Region Provider Router
- Serial -> NY FireWall Serial

## R1 Router on a stick
- Serial -> Connectie naar ROAS 2
- Fa0/1 -> ACSW FE0/1
- FA0/1 -> FWNY FE0/0

## R2 Router on a stick
- Serial -> Connectie naar ROAS 1
- Fa0/1 -> ACSW FE0/1
- FA0/0 -> NYFW FE0/1 

## AS-S1
- FA/1 -> ROAS1 FE0/1

## AS-S2
- FA/1 -> ROAS2 FE0/1

## FW New York
- FA0/0 -> ROAS 1 FE0/0
- FA0/1 -> ROAS 2 FE0/0
