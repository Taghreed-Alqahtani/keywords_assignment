<div dir="rtl">

> continue 

هي بمثابة جملة لتكسر تكرار واحد أي تخطي حدث معين عند تحقق شرط بداخل جملة تكرارية ، 
تستخدم فقط بداخل الجمل التكرارية مثل for , foreach , while, do..while.

مثال :

for (var i = 0; i < 10; i++)
{
    if (i < 5) //شرط لتنفيذ جملة التخطي
    {
        continue;//5 سوف تتخطى أي رقم أقل 
    }
    Console.WriteLine(i);
} 

<div>