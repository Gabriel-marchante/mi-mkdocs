## **1. Elecció de plataformes i llenguatges de programació**

### **Plataformes principals:**
Quan desenvolupem una aplicació mòbil, hem de decidir si serà per:
- **iOS**
- **Android**
- **Ambdues plataformes (multiplataforma)**

### **Llenguatges per al desenvolupament natiu**
- **iOS**: Es recomana utilitzar **Swift** o **Objective-C**.
- **Android**: Es pot fer servir **Kotlin** o **Java**.

```swift
// Exemple de codi Swift per iOS
import UIKit

class ViewController: UIViewController {
    override func viewDidLoad() {
        super.viewDidLoad()
        print("Hola, món!")
    }
}
```

```kotlin
// Exemple de codi Kotlin per Android
package com.example.app

import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity

class MainActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        println("Hola, món!")
    }
}
```

---

## **2. Desenvolupament multiplataforma**
El desenvolupament multiplataforma permet crear aplicacions per a diverses plataformes utilitzant un únic codi base. Hi ha diverses tecnologies populars:

| **Tecnologia**   | **Llenguatge** | **Plataformes suportades**         |
|------------------|----------------|------------------------------------|
| **React Native** | **JavaScript**  | iOS, Android                      |
| **Flutter**      | **Dart**        | iOS, Android, Web, Desktop        |
| **Xamarin**      | **C#**          | iOS, Android, Windows, macOS      |

### **Exemple amb React Native**:
```javascript
import React from 'react';
import { Text, View } from 'react-native';

const App = () => (
  <View>
    <Text>Hola, món!</Text>
  </View>
);

export default App;
```

> **Nota:** Flutter és una altra opció molt popular per a projectes de desenvolupament d'alt rendiment.

---

## **3. Disseny de la interfície d'usuari (UI)**

### **Aspectes a considerar**:
- **Responsivitat**: L'app s'ha d'adaptar a diverses mides de pantalla.
- **Accesibilitat**: Implementar funcions perquè l'app sigui fàcil d'usar per a tothom.
- **UX**: L'experiència de l'usuari ha de ser intuïtiva.

---

## **4. Gestió de dades i bases de dades**

El backend de l'aplicació necessita una gestió eficient de les dades. Algunes bases de dades populars inclouen:

- **SQLite**: Molt utilitzat en aplicacions mòbils.
- **Firebase**: Una opció sense servidor per a apps en temps real.
- **PostgreSQL**: Una base de dades relacional robusta.

### **Exemple d'ús de Firebase**:
```javascript
import firebase from 'firebase/app';
import 'firebase/firestore';

// Configuració de Firebase
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
};

// Inicialitzar Firebase
firebase.initializeApp(firebaseConfig);
const db = firebase.firestore();
```

---

## **5. Proves i desplegament**

### **Proves (Testing)**:
Les proves són essencials per assegurar que l'app funcioni correctament. Es poden fer:
- **Proves unitàries**: Asseguren que les funcions individuals funcionen.
- **Proves d'integració**: Comproven si les diverses parts del sistema treballen conjuntament.

### **Eines de testing**:
- **JUnit** per Android.
- **XCTest** per iOS.
- **Jest** per React Native.

### **Desplegament**:
Un cop finalitzat el desenvolupament, l'app es pot desplegar a:
- **Google Play Store** per a Android.
- **Apple App Store** per a iOS.

---

## **6. Tecnologies addicionals a considerar**
- **APIs RESTful** per comunicar-se amb el servidor backend.
- **GraphQL** per a una gestió més eficient de les dades.
- **CI/CD** (Integració i Distribució Contínua) amb **Jenkins**, **CircleCI** o **GitHub Actions**.

| **Tecnologia**   | **Funció**                                  |
|------------------|---------------------------------------------|
| **Docker**       | Contenidors per facilitar el desplegament   |
| **Kubernetes**   | Orquestració de contenidors                 |
| **Firebase**     | Backend as a Service (BaaS)                 |

---
