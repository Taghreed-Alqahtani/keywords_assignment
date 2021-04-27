<div dir="rtl">

ref

‘ ميزتها أنه "بإمكانك" تغيير قيمتها في الدالة المستدعاه‘
عند تمرير أي متغير مع استخدام ref فأنت تمرره مع الإشاره إليه فإذا حدث تغيير للقيمة في الداله فهو ينعكس على قيمته في الداله التي تم استدعاء الداله بها .

تشترك ref مع in في انه يجب تعريف المتغيرات وإسناد لها قيم قبل إرسالها .

static void Main(string[] args)
{
    int myNum = 10, val=0;
    ProcessNumber(ref myNum, val); 
           
    Console.WriteLine(myNum);
    Console.ReadLine();
}
 
public static void ProcessNumber(ref int num, int val )
{
    num = num + val; // القيمة الجديدة سوف تتغير في الدالة Main
}

<div>
