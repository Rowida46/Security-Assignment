# Secuirity Project

This repository contains an implementation of the following Algorithms.

Encrypt and decryption in [Vigenere](https://github.com/Rowida46/Security-Assignment/blob/main/Python/vigenere.py)

Encrypt and decryption in [Play Fair](https://github.com/Rowida46/Security-Assignment/blob/main/Python/Playfair.py).

Encrypt and decryption in  [Caesar Ciper](https://github.com/Rowida46/Security-Assignment/blob/main/Python/caesar.py).

Encrypt and decryption in  [Autokey](https://github.com/Rowida46/Security-Assignment/blob/main/Python/outokey.py).

To run the script, execute it with the following arguments:

```python
def parse_arguments():
    parser = argparse.ArgumentParser()
    parser.add_argument("-alg", "--algorithm", type= str, required =True,
        choices= ['hill', 'casear', 'outokey', 'playfair', 'vigenere'])
    parser.add_argument('-k', '--key', required= True)
    parser.add_argument("-en", "--encryption", type = str, default ='yes', choices= ["yes" , "no"])
    parser.add_argument("-txt", '--text', type =str)
    args = parser.parse_args()
    return args
```

to run *playfair* with plaintext = `instruments` and key = `Monarchy` excute the following command:

`python main.py -alg playfair -k monarchy -txt instruments `


## To Do

-  [x] PlayFair in js
-  [x] AutoKey in JS
-  [x] Add URL.