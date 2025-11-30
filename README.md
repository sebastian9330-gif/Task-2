## _Ejercicios prácticos Python_

- ### **Con esta código se busca reflejar el movimiento de la tortuga avanzando dejando un rastro, para este ejemplo 10 pasos** 
*Se recomienda ejecutar en la terminal ya que en Jupyter Notebook dentro de VS Code tiende a fallar y reinicia el kernel.*

    def adelante():
    pasos = int(input("¿Cuántos pasos avance? "))
    print("-" * pasos + ">")
    adelante()

**Resultado** 

<img width="871" height="166" alt="image" src="https://github.com/user-attachments/assets/68e231ae-ebf2-499d-8eb3-1ef300d09019" />

---

- ### **Luego buscamos realizar la misma función pero esta vez trazando el avance hacia abajo otros 4 pasos**


        def abajo(pasos):
        for _ in range(pasos):
            print("  " * pasos + "|")   # cada paso hacia abajo 
        print("  " * pasos + "v") # punta de flecha


**Resultado**

<img width="709" height="176" alt="image" src="https://github.com/user-attachments/assets/e41f8d89-4b55-464c-b3e8-9b61931036e9" />

---

- ### **Ahora la tortuga no solo avanza hacia adelante y abajo sino que da un giro de 90 grados a la derecha formando una forma de L a la inversa.**

**Resultado**

<img width="421" height="206" alt="image" src="https://github.com/user-attachments/assets/15d1f87d-ebcc-4230-b950-ce8af0c88a73" />

---

- ### **Con parámetros de “adelante” “abajo” se le da la instrucción de los pasos que debe dar la tortuga.**

        adelante(5) # dibuja la cantidad de paso que da hacia delante encontrandose con la fecha que baja
        abajo(3) # Muestra la cantidad de pasos hacia abajo


**Resultado**

<img width="1053" height="236" alt="image" src="https://github.com/user-attachments/assets/a2dd15d0-6f1d-481d-8bdf-32d9c62463a8" />

---

- ### **Muestra los movimientos “La tortuga” avanzando y trazando la figura bajando escalones.**

        ANCHO = 50
        ALTO = 30
        canvas = [[" " for _ in range(ANCHO)] for _ in range(ALTO)]
        
        # Posición inicial de la tortuga
        x = 0
        y = 0
        
        # funciones
        def resultado():
            for fila in canvas:
                print("".join(fila))
        
        def adelante(pasos):
            global x, y
            for i in range(pasos):
                canvas[y][x] = "-"     # linea horizontal
                x += 1                 # avanzar un paso
            canvas[y][x] = ">"         # flecha final
        
        def abajo(pasos):
            global x, y
            for i in range(pasos):
                y += 1     
                canvas[y][x] = "|" 
            y += 1                      # Hace que las trazado queden juntas y no queden separadas y terminando con la flecha
            canvas[y][x] = "v"
            y += 1                      # Hace que las trazado queden juntas y no queden separadas y terminando con la flecha
    
  ---

        # Escalón 1
        adelante(5)
        abajo(2)
        
        # Escalón 2
        adelante(5)
        abajo(2)
        
        # Escalón 3
        adelante(5)
        abajo(2)
        
        resultado()

**Resultado**

<img width="1266" height="329" alt="image" src="https://github.com/user-attachments/assets/84f0ae90-c1dd-40d8-9109-23fd8188c497" />



### Bibliografias

- [Análisis de código Python. 2025, 30 noviembre ChatGPT](https://chatgpt.com/s/t_692bc18398688191a2844264d69579f6)
- [Análisis de código Python. 2025b, noviembre 30 ChatGPT](https://chatgpt.com/s/t_692bc535e3cc8191a80f909f62a70e96)


    
