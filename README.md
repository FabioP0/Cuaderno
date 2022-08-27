# Cuaderno
Aquí registrare lo que vaya aprendiendo en las clases
___
## Hoja de vida creada en markdown 10-08-2022
[Hoja de vida markdown](https://github.com/FabioP0/hoja_de_vida)
___
## Primer diagrama de flujo
<a href=""><img src="https://github.com/FabioP0/Cuaderno/blob/main/strauml.png?raw=true" alt="fotico" border="0" width="560"></a>
___

## Aquí el primer codigo en visual basic
<a href=""><img src="https://github.com/FabioP0/Cuaderno/blob/main/visual%20basic.png?raw=true" alt="Img" border="0" width="560"></a>
___
## Programa hecho en la clase con esta fecha 26-08-2022
```
Sub impuesto_a_pagar_empresa()
ingreso = InputBox("Isertar los ingresos anuales de la empresa")
    If ingreso >= 1001 And ingreso <= 10000 Then
    impuesto = ((ingreso * 5) / 100)
    MsgBox ("el  impuesto es: " & impuesto)
    Else
        If ingreso >= 10001 And ingreso <= 100000 Then
            impuesto = ((ingreso * 10) / 100)
            MsgBox ("el impuesto es: " & impuesto)
        End If
            If ingreso >= 100001 And ingreso <= 1000000 Then
                impuesto = ((ingreso * 15) / 100)
                MsgBox ("el impuesto es: " & impueto)
            End If
                If ingreso >= 1000001 And ingreso <= 10000000 Then
                    impuesto = ((ingreso * 20) / 100)
                    MsgBox ("el impuesto es: " & impuesto)
                End If
                    If ingreso >= 10000001 Then
                        impuesto = ((ingreso * 25) / 100)
                        MsgBox ("el impuesto es: " & impuesto)
                    End If
                        If ingreso >= 1 And ingreso <= 1000 Then
                            MsgBox ("el impuesto es: " & impuesto)
                        End If
                            If ingreso <= 0 Then
                                MsgBox ("El impuesto es de: " & 0)
                            End If
    End If
End Sub
```
