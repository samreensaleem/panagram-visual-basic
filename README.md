Panagram visual basic 
1. Find if the the input string has all of the alpbhabets; capital or small alike. 
//Pangram
Module Program

    Sub Main()
' *String Manipulation*
' *8) Find if a string is Pangram*

'DELECARATION'
Dim Str1, Str2 As String 
Dim Char1 As Char 
Dim i As Integer 
Dim isPangram As Boolean 

'INITIALISATION' 
Str1 = ""
Str2 = "abcdefghijklmnopqrstuvwxyz"
Char1 = ""
i = 0 
isPangram = True 

'INPUT'
Console.Writeline("Enter string to process: ")
Str1 = Console.Readline
str1=LCase(str1)
'Process't
For i = 1 To Len(Str2)
    Char1 = Mid(Str2, i , 1)
	If InStr(Str1, Char1) = 0 Then isPangram = False 
	Next 
	 
'OUTPUT'
If isPangram = True Then 
   Console.Writeline(Str1 & " Pangram ")
Else 
	Console.Writeline(Str1 & " NOT Pangram.")
	End IF
	console.Readkey()
	
    End Sub 
	End Module
