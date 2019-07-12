# Ud2_Ejemplo14
_Ejemplo 14 de la Unidad 2._ 

Creamos un nuevo estilo para el texto en el fichero _values/styles.xml_:

```
<style name="EstiloTexto">
        <item name="android:layout_width">wrap_content</item>
        <item name="android:layout_height">wrap_content</item>
        <item name="android:textAppearance">?android:textAppearanceLarge</item>
        <item name="android:textStyle">italic</item>
        <item name="android:textColor">@android:color/darker_gray</item>
</style>
```

Y lo aplicamos en los _TextView_ del fichero _activity_main.xml_:

```
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    tools:context=".MainActivity">

    <TextView
        style="@style/EstiloTexto"
        android:text="@string/uno"/>

    <TextView
        style="@style/EstiloTexto"
        android:text="@string/dos"/>

    <TextView
        style="@style/EstiloTexto"
        android:text="@string/tres"/>

</LinearLayout>
```
Observad como se aplica el estilo accediendo al recurso _style_ usando el símbolo @.

Los textos de los _TextView_ se han insertado en el fichero _values/strings.xml_ y accedemos a ellos usando el símbolo @:

```
<resources>
    <string name="app_name">Ud2_Ejemplo14</string>
    <string name="uno">Uno</string>
    <string name="dos">Dos</string>
    <string name="tres">Tres</string>
</resources>
```
