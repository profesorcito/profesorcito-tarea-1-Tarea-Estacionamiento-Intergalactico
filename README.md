[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/tJpLCAHZ)
# **👽 Tarea - Estacionamiento Intergaláctico** 🚀

## **📢🚨 FECHA LÍMITE: 11 de SEPTIEMBRE - 10:00 AM 🚨📢**  
⚠️ **ENTREGAS FUERA DE TIEMPO NO SERÁN ACEPTADAS.**  
✅ **Haz `commit` y `push` antes del plazo y verifica tu entrega en GitHub Classroom.**


## **📖 Historia**  
En el año 3025, los pilotos espaciales que visitan **Marte** deben pagar tarifas de estacionamiento en los **Puertos Orbitales de la Federación Galáctica**.  

El **Consejo de Comercio Espacial** ha establecido un sistema de tarifas, pero debido a las variaciones en la órbita marciana y el tráfico interplanetario, los costos cambian según el **día del ciclo marciano** y **ciertos efectos cósmicos**.  Su proyecto se debe llamar `EstacionamientoIntergalactico`.

## **📜 Reglas del Estacionamiento Espacial**  

### **🚦 Tarifas Base (Lunes a Viernes - Días 1 a 5)**
1. **Primera órbita (1 hora o menos)** → **6 créditos galácticos**  
2. **De 1 a 3 órbitas** → **4 créditos por cada órbita adicional**  
3. **De 3 a 5 órbitas** → **3 créditos por cada órbita adicional**  
4. **Más de 5 órbitas** → **Tarifa fija de 22 créditos**  

### **🌌 Tarifas Especiales (Fines de Semana en Marte - Días 6 y 7)**
- **Sábados y Domingos**: Las tarifas incrementan un **15%** debido a la alta demanda.

### **🛸 Factores Cósmicos (Eventos Aleatorios del Universo)**
1. **Si la suma de los dígitos del número de órbitas es un múltiplo de 3**, el piloto recibe un **descuento del 5%** gracias a la Gravedad Lunar Benefactora.  

### **⛔ Restricciones del Consejo Galáctico**
- **Ninguna nave puede permanecer estacionada más de 24 órbitas marcianas.** Si esto ocurre, el sistema debe mostrar `"ERROR"` y no calcular la tarifa.  

---

## **📌 Entrada**
El programa recibirá **una sola línea de entrada** con dos números enteros separados por un espacio:  
- **H** *(1 ≤ H ≤ 1000)* → Representa las órbitas estacionadas.  
- **D** *(1 ≤ D ≤ 7)* → Representa el día del ciclo marciano (**1 = Lunes, 7 = Domingo**).  

---

## **📌 Salida**  
El programa debe imprimir **un único número** con dos decimales:  
- Si **H > 24**, imprimir `"ERROR"`.  
- En caso contrario, imprimir el costo total a pagar.

---

## **📊 Ejemplo de Entrada y Salida**  

### **Ejemplo 1** (Día de semana sin descuentos)
#### Entrada:
```
2 1
```
#### Salida:
```
10.00
```

---

### **Ejemplo 2** (Fin de semana con incremento)
#### Entrada:
```
5 6
```
#### Salida:
```
23.00
```

---

### **Ejemplo 3** (Descuento por suma de dígitos)
#### Entrada:
```
12 3
```
#### Salida:
```
20.90
```

---

### **Ejemplo 4** (Error por límite excedido)
#### Entrada:
```
25 2
```
#### Salida:
```
ERROR
```

---

## **📜 Notas del Consejo Galáctico** 🛸  
- **El sistema de tarifas debe aplicar correctamente los recargos y descuentos.**  
- **Los cálculos deben realizarse en el orden correcto.**  
- **Los pilotos que estacionen demasiado tiempo serán sancionados.**  

🚀 **¿Eres lo suficientemente hábil para programar este sistema intergaláctico?** 🛸  

---

## **📌 ¿Cómo someter la tarea en GitHub Classroom?**  
### **📝 Pasos para entregar tu código correctamente:**  
1. **Acepta la tarea**.  
2. **Clona tu repositorio** en tu computadora con el siguiente comando (reemplaza `TU_USUARIO` con tu nombre de usuario en GitHub):  
   ```bash
   git clone https://github.com/profesorcito/tarea1-TU_USUARIO.git
   ```
3. **Abre el proyecto en CLion** y escribe tu código en el archivo `main.cpp`.  
4. **Verifica que tu código compile y pase los casos de prueba.**  
5. **Guarda los cambios y súbelos a GitHub:**  
   ```bash
   git add .
   git commit -m "Intento 1"
   git push origin master
   ```
6. **Revisa en GitHub si tu código se ha subido correctamente.**  
7. **Verifica los resultados en GitHub Classroom**, donde el sistema de autograding evaluará tu código automáticamente.  

⚠️ **IMPORTANTE:**  
- **No cambies el nombre del repositorio ni del archivo principal (`main.cpp`).**  
- **Asegúrate de hacer `commit` y `push` antes de la fecha límite.**  
- **Si encuentras errores en el autograder, revisa tu salida y ajústala según los ejemplos dados.**  

---

### **💻 Esqueleto del Código en C++ (Incompleto para que los estudiantes lo completen)**  
```cpp
#include <iostream>

using namespace std;

// TODO: Implementar función para calcular la suma de los dígitos de un número
int sumaDigitos(int n) {
    // Completa esta función
}

// TODO: Implementar la lógica para calcular la tarifa
double calcularTarifa(int horas, int dia) {
    const double TARIFA_PRIMERA_HORA = 6.00;
    const double TARIFA_1_A_3 = 4.00;
    const double TARIFA_3_A_5 = 3.00;
    const double TARIFA_FIJA = 22.00;
    const int LIMITE_HORAS = 24;
    const double INCREMENTO_FIN_SEMANA = 1.15;
    const double DESCUENTO_DIGITOS = 0.95;

    // Validar límite de horas
    if (horas > LIMITE_HORAS) {
        return -1;
    }

    double totalPagar = 0.0;

    // TODO: Implementar la lógica para calcular la tarifa base
    if (horas == 1) {
        // Completa aquí
    } else if (horas > 1 && horas <= 3) {
        // Completa aquí
    } else if (horas > 3 && horas <= 5) {
        // Completa aquí
    } else {
        // Completa aquí
    }

    // TODO: Aplicar incremento si es fin de semana
    if (/* Completa esta condición */) {
        totalPagar *= INCREMENTO_FIN_SEMANA;
    }

    // TODO: Aplicar descuento si la suma de los dígitos es múltiplo de 3
    if (/* Completa esta condición */) {
        totalPagar *= DESCUENTO_DIGITOS;
    }

    return totalPagar;
}

int main() {
    int horas, dia;

    // Leer los valores de entrada
    cin >> horas >> dia;

    double resultado = calcularTarifa(horas, dia);
    if (resultado == -1) {
        cout << "ERROR" << endl;
    } else {
        printf("%.2f\n", resultado);
    }

    return 0;
}
```

---

## **📌 ¿Qué debes hacer?**
1. **Completar la función `sumaDigitos()`** para calcular la suma de los dígitos de un número.  
2. **Completar la lógica dentro de `calcularTarifa()`** para determinar el costo base según el tiempo estacionado.  
3. **Rellenar la condición para aplicar el recargo de fin de semana** (`D == 6` o `D == 7`).  
4. **Rellenar la condición para aplicar el descuento cuando la suma de los dígitos de `H` sea múltiplo de 3**.  
5. **Probar su código con los ejemplos de entrada/salida para verificar que funcione correctamente.**  

---
