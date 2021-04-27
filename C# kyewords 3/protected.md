<div dir="rtl">

> protected 

تصنف من ضمن access modifier أي تتحكم في الوصول إلى قيم المتغيرات , protectd تسمح بالوصول اذا كانت في نطاق الكلاس أو مايرث منه .

class A
{
    protected int x = 123;
}

class B : A
{
    static void Main()
    {
        var a = new A();
        var b = new B();
        b.x = 10; //الوصول إلى قيمة x من خلال الكائن B لأنه يرث من A
    }
}

<div>