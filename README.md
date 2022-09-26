# Cuaderno
## Regristro de las clase de las clases 
___
## Hoja de vida creada en markdown 10-08-2022
[Hoja de vida markdown](https://github.com/FabioP0/hoja_de_vida)
___
## Primer diagrama de flujo
<a href=""><img src="https://github.com/FabioP0/Cuaderno/blob/main/strauml.png?raw=true" alt="fotico" border="0" width="560"></a>

## Primer codigo en visual basic
<a href=""><img src="https://github.com/FabioP0/Cuaderno/blob/main/visual%20basic.png?raw=true" alt="Img" border="0" width="560"></a>
___
## Porgrama aprobación nota estudiante 24-08-2022
```
Sub aprobo_estudiante()
   nom = InputBox("Escriba el nombre del alumno")
   par = Int(InputBox ("Escriba la nota del parcial"))
   exa = Int(InputBox ("Escriba nota del examen final"))
   pra = Int(InputBox ("Escriba promedio de practicas"))
   nota = ((exa * 2) + par + pra) / 3
   If nota = 6 Then
      MsgBox ("El nombre del alumno es: " & nom)
      MsgBox ("El alumno con nombre: " & nom & " aprobo con esta nota: " & nota)
   Else
      MsgBox ("No aprobo")
   End If 
End Sub
```
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
## Impuesto empresa con estructura Select Case
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
## Porgrama utilizando el ciclo while
```
Sub aporte_estudiantes()
    aporte = 0
    noapor = 0
    masde = 0
    i = 0
    est = 0
    While i < 3000000
        aporte = Int(InputBox("Ingrese cuanto va a aportar"))
        If aporte < 0 Then
            MsgBox ("Error, el valor que ingreso no es valido")
        Else
            If aporte = 0 Then
                MsgBox ("El estudiante no aporto")
                noapor = noapor + 1
            End If
            If aporte > 0 Then
                i = aporte + i
                est = est + 1
            End If
            If aporte > 10000 Then
                masde = masde + 1
            End If
        End If
    Wend
    prom = i / est
    MsgBox ("El total aportado fue de: " & "$" & i)
    MsgBox ("Estudiantes que aportaron: " & est)
    MsgBox ("Estudiantes que aportaron más de $10.000: " & masde)
    MsgBox ("Estudiantes que no aportaron: " & noapor)
    MsgBox ("El promedio del valor de los estudiantes que aportaron es de: " & "$" & prom)
End Sub
```
