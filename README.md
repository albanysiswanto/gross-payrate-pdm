# Gross Salary

adalah program yang dibuat untuk menyelesaikan tugas Program Design Method menggunakan NetBeans

## Logic

```java
private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // Exit
        dispose();
    }                                        

    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        if(hourTxt.getText().isEmpty() || payTxt.getText().isEmpty()){
            JOptionPane.showMessageDialog(null, "Hours or Pay Rate is Empty", "Errors", JOptionPane.ERROR_MESSAGE);
        }else{
            double hour = Double.parseDouble(hourTxt.getText()),
                    payRate =  Double.parseDouble(payTxt.getText()),
                    total;
            
            total = hour * payRate;
            showTotal.setText("$" + total);
        }
    }  
```

## Penjelasan

```java
if(hourTxt.getText().isEmpty() || payTxt.getText().isEmpty()){
            JOptionPane.showMessageDialog(null, "Hours or Pay Rate is Empty", "Errors", JOptionPane.ERROR_MESSAGE);
        }
```
Code diatas adalah pengodisian ketika Text Field Hours & PayRate Empty atau kosong maka akan memunculkan sebuah alert dengan message "Hours or Pay Rate is Empty", Title "Errors", dan messageType "JOptionPane.ERROR_MESSAGE".

```java
else{
            double hour = Double.parseDouble(hourTxt.getText()),
                    payRate =  Double.parseDouble(payTxt.getText()),
                    total;
            
            total = hour * payRate;
            showTotal.setText("$" + total);
        }
```
Code diatas adalah pengodisian ketika Text Field tidak kosong maka menjalankan code diatas. Pengondisian diatas diawali dengan mengkonversi text ke double agar dapat dikalikan antara Hours & PayRate.
