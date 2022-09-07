# Cuaderno
## Regristro de las clase de las clases 
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
## Programa impuesto empresa 26-08-2022
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
## Programa impuesto empresa con estructura Select Case
```
Sub sena()
    ingreso = Int(InputBox("Escriba los ingresos anuales de la empresa"))
        Select Case ingreso
            Case 0 To 1000
                MsgBox ("El impuesto a pagar es: " & ingreso)
                Case 1001 To 10000
                    impuesto = ((ingreso * 5) / 100)
                    MsgBox ("El impuesto a pagar es: " & impuesto)
                Case 10001 To 100000
                    impuesto = ((ingreso * 10) / 100)
                    MsgBox ("El impuesto a pagar es: " & impuesto)
                Case 100001 To 1000000
                    impuesto = ((ingreso * 15) / 100)
                    MsgBox ("El impuesto a pagar es: " & impuesto)
                Case 1000001 To 10000000
                    impuesto = ((ingreso * 20) / 100)
                    MsgBox ("El impuesto a pagar es: " & impuesto)
                Case Else
                    impuesto = ((ingreso * 25) / 100)
                    MsgBox ("El impuesto a pagar es: " & impuesto)
        End Select
End Sub
```
___
## Programa estudiantes 31-08-2022
```
Sub estudiante()
    cont = 0
    acum = 0
    masde = 0
    cant = Int(InputBox("Ingrese la cantidad de estudiantes que aportaron de los 7500"))
        For i = 1 To cant
            aporto = Int(InputBox("Ingrese la cantidad que aporto el estudiante"))
            cont = cont + 1
            acum = acum + aporto
            noapor = 7500 - cant
            prom = acum / cont
                If aporto > 10000 Then
                    masde = masde + 1
                End If
        Next i
    MsgBox ("Cantidad de estudintes que aporto: " & cant)
    MsgBox ("total recaudado: " & acum)
    MsgBox ("El numero de estudiantes que no aporto: " & noapor)
    MsgBox ("Valor recaudo promedio: " & prom)
    MsgBox ("Los estudiantes que aportaron mas de 10.000 fueron: " & masde)
End Sub
```
___
Sub INICIO()
   InputBox ("escriba el nombre del alumno "), f
   InputBox ("escriba nota parcial "), b
   InputBox ("escriba nota del examen final "), m
   InputBox ("escriba promedio de practicas "), j

   bm = (f + b + m + j) / 4
   
   If bm = 6 Then
      MsgBox ("el nombre es : "), f
      MsgBox ("el promedio final es : "), bm
      MsgBox ("aprobado ")
   Else
      MsgBox ("desaprobado ")
   End If
   
End Sub
```
