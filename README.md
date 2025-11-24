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


## CSW2
- Fa0/1 -> L2-S1 Fa0/2
- Fa0/3 -> L2-S2 Fa0/4
- Fa0/23 -> CSW1 Fa0/23
- Fa0/24 -> CSW1 Fa0/24

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
-
-
-

## R1 Router on a stick
-
-
-

## R2 Router on a stick
-
-
-

## AS-S1
-
-
-

## AS-S2
-
-
-
