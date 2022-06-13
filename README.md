## Week1 HomeWork

1)	Ekrana 10 kez “Hello World!” yazdır.

```
var i = 0
while i < 10 {
    
    print("Hello World")
    i += 1
} 
```

2)	43 sayısına kadar olan TEK sayıları print et
```
for i in 1..<43 {
    if i % 2 == 1 {
        print(i)
    }
    
 
}
```

3)	Dışarıdan aldığı metnin soluna “TR-” ekleyip döndüren metot
```
func addTr(Word : String) {
     print("TR-\(Word)")
    
}
```

4)	Dışarıdan girilen bir sayının rakamları toplamını bulan program.  ( Örneğin kullanıcı 431 girdiğinde sonuç: 8 olacak)
```
var sum = 0

func SumOfDigits(number:Int)->Int {
    
    if number > 0 {
        sum += (number % 10)
        return SumOfDigits(number:number / 10)
    }

    return sum
}
```

5)	 Doğduğum günden bugüne kaç gün geçtiğini gösteren metot? Dışarıdan date alacak int dönüyor. 
```
func Date(number:Int) -> Int {
    
 var difference = 2022 - number
 var result = difference * 365
    return result


}
```

6)	Dışarıdan girilen üç sayıdan en büyüğünü bulan metot
```
func maxNumber(_ x: Int, _ y: Int, _ z: Int) -> Int {
    if x > y, x > z
    {
        return x
    }
    else if y > z, y > x
    {
        return y
    }
    else if z > y, z > x
    {
        return z
    }
    else if x == y, y > z
    {
        return x
    }
    else if y == z, z > x
    {
        return y
    }
    else
    {
        return x
    }
}
```

7)	Dışarıdan bir metin alan aldığı metnin sadece ilk üç harfini döndüren fonksiyon.
```
func text(message : String) -> String  {
    return String(message.prefix(3))
   



}
```

8)	Dışarıdan bir isim dizisi alan ve isimleri tek tek print eden fonksiyon
```
func name(text : [String])   {
   
    for character in text {
        
            
            print(character)
        }
       
    }
```

9)	 Dışarıdan bir isim dizisi alan, ismin uzunluğu 4 den büyükse print eden fonksiyon.
```
func text(charArr : [String]) {
    
    for i in charArr {
        if i.count > 4 {
            print(i)
        } else {
            print("")
        }
    }
}
```
10)	 Dışarıdan bir metin alan ve aldığı metinde kaç adet "e" harfi olduğunu söyleyen fonksiyon.
```
func text(str : String) {
    var i = 0
    for a in str {
        if a == "e" {
            i += 1
            
        }
       
        
    }
    print(i)
}
```
11)	 Dışarıdan bir metin alan aldığı metnin sadece ilk harfini büyük diğer harflerini küçük yazacak şekilde yeni bir metin oluşturarak dönen fonksiyon.
```
func text(str : String) -> String {
    return str.capitalized
    }
```

