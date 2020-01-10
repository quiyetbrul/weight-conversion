Public Class Form1
    Private Sub Button3_Click(sender As Object, e As EventArgs) Handles Button3.Click
        Application.Exit()

    End Sub

    Private Sub Button2_Click(sender As Object, e As EventArgs) Handles Button2.Click
        TextBox1.Clear()
        TextBox1.Focus()
        Label3.Text = ""

    End Sub

    Private Sub Button1_Click(sender As Object, e As EventArgs) Handles Button1.Click

        If TextBox1.Text = "" Then
            MessageBox.Show("Please enter your weight in pounds.")
            With TextBox1
                .Focus()
                .SelectAll()
            End With
        ElseIf IsNumeric(TextBox1.Text) = False Then
            MessageBox.Show("Invalid input. Please enter your weight " &
                            "in pounds with numeric value.")
        End If


        Dim Venus As Decimal
        Venus = 0.907 * TextBox1.Text
        Dim Mars As Decimal
        Mars = 0.377 * TextBox1.Text
        Dim kg As Decimal
        kg = 0.454 * TextBox1.Text

        If RadioButton1.Checked = True Then

            Label3.Visible = True
            Label3.Text = "Your weight in Venus is " & (Venus) & " lbs or" &
                " " & kg & " kg."

        ElseIf RadioButton2.Checked = True Then
            Label3.Text = Mars * TextBox1.Text
            Label3.Visible = True
            Label3.Text = "Your weight in Mars is " & (Mars) & " lbs or" &
               " " & kg & " kg."
        Else
            MessageBox.Show("Choose a planet to convert your weight to.")

        End If

    End Sub

    Private Sub Form1_Load(sender As Object, e As EventArgs) Handles MyBase.Load
        Label3.Visible = False
    End Sub
End Class



