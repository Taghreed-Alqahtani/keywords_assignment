<div dir="rtl">

> in 

لها عدة استخدامات مثل تمرير المتغيرات الى دوال وجملة foreach و from , join في LINQ.

‘ميزتها أنك "لا تستطيع" تغيير قيمتها في الدالة المستدعاه‘

غالبا تستخدم لتحسين أداء البرنامج.

تشترك ref مع in في انه يجب تعريف المتغيرات وإسناد لها قيم قبل إرسالها .

مثال في تمرير المتغيرات :

{
int readonlyArgument = 44;
InArgExample(readonlyArgument);
Console.WriteLine(readonlyArgument);
}
void InArgExample(in int number)// لإستخدام قيمتها فقط 
{
}

مثال في جملة foreach:

foreach(var item in collection)
{

}

<div>
