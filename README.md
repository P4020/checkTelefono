# checkTelefono
### Descrizione Esercizio
#### Nel seguente compito dovevamo trovare se il vettore stringa fosse un numero italiano controllando i numeri iniziale della stringa in 3 modi differenti : 
#### 1- Con il +39 e deve essere lunga esattamente 13. 
#### 2- Con lo 0039 e deve essere esattamente lunga 14.
#### 3- Oppure con il 3 e deve essere lunga esattamente 10.
### Codice
```
  foreach (string stringa in input)
        {
            // Verifica se la stringa inizia con +39 ed è lunga 13
            if (Regex.IsMatch(stringa, @"^\+39\d{11}$"))
            {
                return stringa;
            }
            // Verifica se la stringa inizia con 0039 ed è lunga 14
            else if (Regex.IsMatch(stringa, @"^0039\d{11}$"))
            {
                return stringa;
            }
            // Verifica se la stringa inizia con 3 ed è lunga 10
            else if (Regex.IsMatch(stringa, @"^3\d{9}$"))
            {
                return stringa;
            }
        }
```
