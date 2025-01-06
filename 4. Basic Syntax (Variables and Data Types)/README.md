## Sintaks Dasar: Variabel dan Tipe Data

Berikut ini adalah program sederhana untuk mendeklarasikan variabel dan tipe data di Go:

## Variabel
- **Deklarasi Biasa**: Menggunakan `var`.
- **Deklarasi Cepat**: Menggunakan `:=`.

Contoh:
```go
var nama string = "Budi"
umur := 20
```
## Tipe Data 
- **String**: `string`
- **Integer**: `int`, `int8`, `int16`, `int32`, `int64`
- **Floating-point**: `float32`, `float64`
- **Boolean**: `bool`

#### String
Berikut merupakan contoh penggunaan dari String
```go
package main

import "fmt"

func main() {
    // Deklarasi String
    var firstName string = "John"       // Deklarasi dengan var
    lastName := "Doe"                   // Deklarasi cepat
    fullName := firstName + " " + lastName // Menggabungkan string

    // Output
    fmt.Println("Full Name:", fullName) // Output: Full Name: John Doe

    // Panjang String
    fmt.Println("Length of fullName:", len(fullName)) // Output panjang string

    // Akses karakter dalam string
    fmt.Println("First letter of fullName:", string(fullName[0]))
}
```
 Output:

#### Integer
Berikut merupakan contoh penggunaan dari Integer
 ```go
package main

import "fmt"

func main() {
    // Deklarasi Integer
    var age int = 25                    // Integer default
    var smallNumber int8 = 100          // Integer 8-bit
    var mediumNumber int16 = 1000       // Integer 16-bit
    var largeNumber int64 = 1000000000  // Integer 64-bit

    // Output
    fmt.Printf("Age: %d\nSmall: %d\nMedium: %d\nLarge: %d\n", age, smallNumber, mediumNumber, largeNumber)

    // Operasi Matematika
    total := int(smallNumber) + age // Konversi tipe data
    fmt.Println("Total (smallNumber + age):", total)

    // Modulus
    fmt.Println("Modulus (age %% 7):", age%7)
}
```
#### Boolean
Berikut merupakan contoh penggunaan dari Boolean
```go
package main

import "fmt"

func main() {
    var isGoFun bool = true
    fmt.Println(isGoFun) // Output: true
}
```
Output:
