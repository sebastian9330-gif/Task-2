## Ejercicios prácticos Python

Con esta código se busca reflejar el movimiento de la tortuga avanzando dejando un rastro, para este ejemplo 10 pasos. 
Se recomienda ejecutar en la terminal ya que en Jupyter Notebook dentro de VS Code tiende a fallar y reinicia el kernel.

def adelante():

    pasos = int(input("¿Cuántos pasos avance? "))
    
    print("-" * pasos + ">")

adelante()

**Resultado** 

<img width="871" height="166" alt="image" src="https://github.com/user-attachments/assets/68e231ae-ebf2-499d-8eb3-1ef300d09019" />

---

Luego buscamos realizar la misma función pero esta vez trazando el avance hacia abajo otros 4 pasos


def abajo(pasos):

    for _ in range(pasos):
    
        print("  " * pasos + "|")   # cada paso hacia abajo 
        
    print("  " * pasos + "v") # punta de flecha


**Resultado**

<img width="709" height="176" alt="image" src="https://github.com/user-attachments/assets/e41f8d89-4b55-464c-b3e8-9b61931036e9" />

---

Ahora la tortuga no solo avanza hacia adelante y abajo sino que da un giro de 90 grados a la derecha formando una forma de L a la inversa.

**Resultado**

<img width="421" height="206" alt="image" src="https://github.com/user-attachments/assets/15d1f87d-ebcc-4230-b950-ce8af0c88a73" />

---

Con parámetros de “adelante” “abajo” se le da la instrucción de los pasos que debe dar la tortuga.

adelante(5) # dibuja la cantidad de paso que da hacia delante encontrandose con la fecha que baja

abajo(3) # Muestra la cantidad de pasos hacia abajo 


**Resultado**

<img width="1053" height="236" alt="image" src="https://github.com/user-attachments/assets/a2dd15d0-6f1d-481d-8bdf-32d9c62463a8" />

---








    
