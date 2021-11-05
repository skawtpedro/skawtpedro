import random 

"""creamos nuestra baraja"""
cartas = ["A","2","3","4";"5";"6";"7";"S","C","R"]
figuras = ["oros","copas","espadas","bastos"]
baraja = []

"""lista vacia"""
for i in cartas:
    for p in figuras:
        carta = "{} de {}".format(t,p)
        baraja.append(carta)
        
random.suffle(baraja)

for i in range(0,52,4):
    for j in range(4):
        print("{:14}".format(baraja[i+j]), end="")
    print()
    
print()

#repartiendo cartas a jugadores 
jugadores = [[],[],[],[]]

for i in range(5):
    for j in range(4):
    jugadores[j].append(baraja.pop(0))

# mostrando las cartas de cada jugador
jugadores = [jugador1, jugador2, jugador3, jugador4]

for i in range(4):
    print("Jugador {}: ".format(i+1))
    for j in range(5):
        print("{:16}".format(jugadores[i][j]), end="")
    print()
    
print()

#Mostrando las cartas

for i in range(0,32,4):
    for j in range(4):
        print("{:14}".format(baraja[i+j]), end="")
    print()
        








