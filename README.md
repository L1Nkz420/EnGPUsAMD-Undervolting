# AMD GPU Power Profile (Undervolting)

Perfil personalizado de GPU AMD mediante archivo XML para ajuste de:
- P-States
- Voltajes
- Frecuencias
- Curva de ventilador
- Parámetros de energía

Este perfil está orientado a **reducir temperaturas y consumo** manteniendo estabilidad.

---

## Información de la GPU

- Fabricante: AMD
- DevID: 6FDF
- RevID: EF
- Tipo de ajuste: Undervolt / tuning manual
- Uso recomendado: Gaming / uso prolongado

---

## Archivo de configuración

El siguiente archivo XML define los estados de energía y control térmico de la GPU.

> **Nota:** Este código no se ejecuta desde GitHub.  
> Solo se documenta aquí. El archivo real debe guardarse como `.xml`.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SYSTEM>
    <GPU DevID="6FDF" RevID="EF">
        <PPW Value="1"/>

        <FEATURE ID="100" Enabled="0">
            <STATES>
                <STATE ID="0" Enabled="False" Value="0"/>
            </STATES>
        </FEATURE>

        <FEATURE ID="101" Enabled="0">
            <STATES>
                <STATE ID="0" Enabled="True" Value="0"/>
            </STATES>
        </FEATURE>

        <FEATURE ID="102" Enabled="15">
            <STATES>
                <STATE ID="0" Enabled="True" Value="0"/>
            </STATES>
        </FEATURE>

        <FEATURE ID="4" Enabled="False">
            <STATES>
                <STATE ID="0" Enabled="True" Value="300"/>
                <STATE ID="1" Enabled="True" Value="600"/>
                <STATE ID="2" Enabled="True" Value="900"/>
                <STATE ID="3" Enabled="True" Value="1077"/>
                <STATE ID="4" Enabled="True" Value="1145"/>
                <STATE ID="5" Enabled="True" Value="1191"/>
                <STATE ID="6" Enabled="True" Value="1231"/>
                <STATE ID="7" Enabled="True" Value="1244"/>
            </STATES>
        </FEATURE>

        <FEATURE ID="12" Enabled="True">
            <STATES>
                <STATE ID="0" Enabled="True" Value="750"/>
                <STATE ID="1" Enabled="True" Value="750"/>
                <STATE ID="2" Enabled="True" Value="806"/>
                <STATE ID="3" Enabled="True" Value="943"/>
                <STATE ID="4" Enabled="True" Value="1012"/>
                <STATE ID="5" Enabled="True" Value="1062"/>
                <STATE ID="6" Enabled="True" Value="1106"/>
                <STATE ID="7" Enabled="True" Value="1125"/>
            </STATES>
        </FEATURE>

        <FEATURE ID="5" Enabled="False">
            <STATES>
                <STATE ID="0" Enabled="True" Value="300"/>
                <STATE ID="1" Enabled="True" Value="1000"/>
                <STATE ID="2" Enabled="True" Value="1750"/>
            </STATES>
        </FEATURE>

        <FEATURE ID="13" Enabled="True">
            <STATES>
                <STATE ID="0" Enabled="True" Value="750"/>
                <STATE ID="1" Enabled="True" Value="800"/>
                <STATE ID="2" Enabled="True" Value="900"/>
            </STATES>
        </FEATURE>

        <FEATURE ID="9" Enabled="True">
            <STATES>
                <STATE ID="0" Enabled="True" Value="0"/>
                <STATE ID="1" Enabled="True" Value="0"/>
                <STATE ID="2" Enabled="True" Value="900"/>
            </STATES>
        </FEATURE>

        <FEATURE ID="22" Enabled="True">
            <STATES>
                <STATE ID="0" Enabled="True" Value="30"/>
                <STATE ID="1" Enabled="True" Value="20"/>
                <STATE ID="2" Enabled="True" Value="50"/>
                <STATE ID="3" Enabled="True" Value="35"/>
                <STATE ID="4" Enabled="True" Value="60"/>
                <STATE ID="5" Enabled="True" Value="50"/>
                <STATE ID="6" Enabled="True" Value="70"/>
                <STATE ID="7" Enabled="True" Value="60"/>
                <STATE ID="8" Enabled="True" Value="85"/>
                <STATE ID="9" Enabled="True" Value="75"/>
            </STATES>
        </FEATURE>
    </GPU>
</SYSTEM>

By L1Nkz.
