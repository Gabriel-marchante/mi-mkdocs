# Identificació dels Espais de Noms en Documents `AndroidManifest.xml`

L'**`AndroidManifest.xml`** és un fitxer essencial en qualsevol aplicació Android, ja que defineix la configuració de l'aplicació, incloent-hi els seus components, permisos i altres detalls importants. Un dels aspectes fonamentals és la gestió dels **espais de noms**, que són una forma d'organitzar i categoritzar les etiquetes XML i atributs associats.

## Què és un Espai de Noms?

Un espai de noms XML és un identificador que evita conflictes de noms entre els elements XML. Això és especialment útil en projectes grans o complexos, on diferents biblioteques poden utilitzar les mateixes etiquetes o noms d'elements. Els espais de noms s'especifiquen amb l'atribut `xmlns`.

### Exemples d'Espais de Noms en `AndroidManifest.xml`

A continuació, es mostra un exemple de com es declaren els espais de noms en un document **`AndroidManifest.xml`**:

```xml
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.example.app">
    
    <!-- Declaració de l'activitat principal -->
    <application
        android:allowBackup="true"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name">
        
        <activity android:name=".MainActivity">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>
</manifest>
```

En aquest exemple:

- **`xmlns:android="http://schemas.android.com/apk/res/android"`**: Es tracta de l'espai de noms per defecte utilitzat per Android, que identifica els atributs i elements que pertanyen a l'API d'Android.
- **`package="com.example.app"`**: Fa referència al paquet de l'aplicació.

### Espais de Noms en XML

Els espais de noms normalment s'utilitzen en fitxers XML per diferenciar elements i atributs provinents de diferents orígens. Això és útil quan es combinen múltiples esquemes o es fa ús de diferents biblioteques que poden compartir noms d'elements o atributs.

#### Estructura bàsica d'un espai de noms

- `xmlns:prefix="URI"`: El prefix associat a l'espai de noms.
- `URI`: L'URI és la referència que identifica de manera única l'espai de noms.

Per exemple:

```xml
<root xmlns:android="http://schemas.android.com/apk/res/android">
    <element android:attribute="value" />
</root>
```

En aquest cas, `android` és el prefix i s'utilitza per referenciar atributs com `android:attribute`.

### Taula d'atributs associats a espais de noms comuns

| Prefix         | URI                                               | Descripció                          |
|----------------|---------------------------------------------------|-------------------------------------|
| **android**    | `http://schemas.android.com/apk/res/android`       | Espai de noms d'Android             |
| **tools**      | `http://schemas.android.com/tools`                | Espai de noms per eines de disseny  |
| **app**        | `http://schemas.android.com/apk/res-auto`         | Espai de noms personalitzat         |

## Com es poden combinar múltiples Espais de Noms?

És possible combinar múltiples espais de noms dins del mateix document XML. Aquí tens un exemple:

```xml
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hola, món!"
        app:fontFamily="sans-serif" />
</LinearLayout>
```

### Explicació

1. **Espai de noms `android`**: Es fa servir per tots els atributs estàndard d'Android (`android:layout_width`, `android:layout_height`).
2. **Espai de noms `app`**: S'utilitza per atributs personalitzats o de biblioteques de tercers, com el `app:fontFamily`.
3. **Espai de noms `tools`**: Aquest espai de noms és només per a ús de desenvolupament i no afecta el funcionament de l'aplicació en producció. El `tools:context` és utilitzat per a suggeriments en l'entorn de desenvolupament.