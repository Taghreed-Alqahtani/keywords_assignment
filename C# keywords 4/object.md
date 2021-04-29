<div dir="rtl">

> object

هي عبارة عن مساحة في الذاكرة تشير إلى كائن محدد ، البرنامج يستطيع إنشاء عدة كائنات من نفس الكلاس.
من خلال الكائن أستطيع الوصول الى الخصائص والدوال العامه في الكلاس ولذلك تسمى C# لغة كائنية لأن البرنامج مكون من عدة كائنات تتفاعل مع بعضها .
ممكن أن يكون الكائن من كلاس او ستركت 'struct'
عند انشاء كائن من كلاس ثم إنشاء متغير يشير إلى نفس الكائن فهو في الواقع فقط يشير إليه في الذاكره ،ولكن عند إنشاء متغير من struct فكل متغير يحتفظ بنسخة جديده خاصه فيه .

<div>

```C#
public class animal
{
    public string Name { get; set; }
    public string Color { get; set; }
    public Person(string name, string color)
    {
        Name = name;
        Color = color;
    }
}

class Program
{
    static void Main()
    {
        animal cat =new animal("luna","white");// كائن اسمه cat له خصائصه الخاصة فيه 
    }
}

//////////////

public struct Person
{
    public string Name;
    public int Age;
    public Person(string name, int age)
    {
        Name = name;
        Age = age;
    }
}

public class Application
{
    static void Main()
    {
        Person p1 = new Person("Alex", 9);
        
        Person p2 = p1; // p2 انشأ نسخه جديده
    }
}

```