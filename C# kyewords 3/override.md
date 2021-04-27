<div dir="rtl">

> override

تكتب مع الدالة الموروثة من الكلاس الأم لإنشاء تعريف جديد خاص بالكلاس الحالي ،لا يمكن كتابة static , new ,virtual معها في نفس الدالة.
يجب ان تكون الداله في الكلاس الأم إما abstract او virtual أو override


public class Users 
{
    public virtual void GetInfo()
    {
       Console.WriteLine("Base Class");
    }
}

public class Details: Users // كلاس details يرث دالة getinfo من users
{
    public override void GetInfo() // تغيير جملة الطباعه بداخلها
    {
       Console.WriteLine("Derived Class");
    }
}


<div>