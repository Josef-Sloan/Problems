# Problems
/Users/josefsloan/Projects/Battleships/Battleships/CSC: Error CS5001: Program does not contain a static 'Main' method suitable for an entry point (CS5001) (Battleships)

This is a project for my computer science class in school and I don't understand the error.

I'm using General VBNet on Mac 


Imports System.IO

Module Module1

Sub Main()

Dim BattleshipArray(11) as string 
Dim FILE_NAME As String = "/Users/josefsloan/Desktop"

BattleshipArray(0) = "j"
BattleshipArray(1) = "i"
BattleshipArray(2) = "l"
BattleshipArray(3) = "m"
BattleshipArray(4) = "n"
BattleshipArray(5) = "o"
BattleshipArray(6) = "p"
BattleshipArray(7) = "q"
BattleshipArray(8) = "r"
BattleshipArray(9) = "s"
BattleshipArray(10) = "t"

Dim objwriter as New System.IO.StreamWrite(FILE_NAME, False)

If System.IO.File.Exists(FILE_NAME) = True Then

For i as Integer = 0 to 11 

objwriter.writeline(BattleshipArray(i))

Next

objwriter.Close()

MsgBox("Text Writting to File")

Else 

MsgBox("File does not Exist")

End If

End Sub

End Module
