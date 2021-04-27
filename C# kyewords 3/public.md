<div dir="rtl">

> public 

تصنف من ضمن access modifier أي تتحكم في الوصول
وهي تسمح بالوصول الى المتغيرات والدوال داخل الكلاس ومايرث منه وخارج الكلاس

```C#
public class User // كلاس public
    {
        // متغيرات public
       public string Name; 
       public string Location;
       public int Age;
       public void GetUserDetails() // دالة public
       {
           Console.WriteLine("Name: {0}", Name);
           Console.WriteLine("Location: {0}", Location);
           Console.WriteLine("Age: {0}", Age);
       }
    }

```
<div>
