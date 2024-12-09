# Exemples de Traducció d'Ordres en Python, C++, i Java

En aquesta secció es mostren exemples bàsics de com executar programes en Python, C++ i Java utilitzant les ordres `python3`, `cc`, `java` i `javac`.

## **Python3**
Per executar un programa en Python, podem utilitzar l'ordre **`python3`**.

### **Exemple de codi Python:**
```python
# Hola món en Python
print("Hola món!")
```

### **Com executar-ho:**
Per executar aquest codi, guardem-lo en un fitxer amb extensió `.py` (per exemple, `hola.py`), i després executem:

```bash
python3 hola.py
```

---

## **C++**
En C++, primer cal compilar el codi utilitzant l'ordre **`cc`**, i després executar l'arxiu resultant.

### **Exemple de codi C++:**
```cpp
// Hola món en C++
#include <iostream>
using namespace std;

int main() {
    cout << "Hola món!" << endl;
    return 0;
}
```

### **Com compilar i executar:**
Guardem el codi en un fitxer amb extensió `.cpp` (per exemple, `hola.cpp`), i després executem:

```bash
cc hola.cpp -o hola
./hola
```

---

## **Java**
En Java, primer compilem el codi amb **`javac`** i després l'executem amb **`java`**.

### **Exemple de codi Java:**
```java
// Hola món en Java
public class Hola {
    public static void main(String[] args) {
        System.out.println("Hola món!");
    }
}
```

### **Com compilar i executar:**
Guardem el codi en un fitxer amb extensió `.java` (per exemple, `Hola.java`), i després executem:

```bash
javac Hola.java
java Hola
```

---

## **Taula comparativa de les ordres**
A continuació es mostra una taula que resumeix les ordres necessàries per executar un programa en cadascun dels llenguatges.

| Llenguatge | Com compilar | Com executar |
|------------|--------------|--------------|
| Python     | No aplicable  | `python3 hola.py` |
| C++        | `cc hola.cpp -o hola` | `./hola` |
| Java       | `javac Hola.java` | `java Hola` |

---
## **Enllaços útils**

- [Documentació oficial de Python](https://docs.python.org/3/)
- [Documentació oficial de C++](https://en.cppreference.com/w/)
- [Documentació oficial de Java](https://docs.oracle.com/en/java/)

---