<div dir="rtl">

> this

هي كلمة تستخدم للإشاره إلى الكلاس الحالي وأيضا تستخدم في دوال extension

<div>

```C#
المثال الاول 
public class Employee
{
    private string name;
    public Employee(string name)
    {
        this.name = name;// تشير الى المتغير المعرف في الكلاس الحالي
    }
}

المثال الثاني 
 
        public static bool isCapital(this string text)// أصبحت isCapital من الميثود التابعه للنصوص
        {
            return char.IsUpper(text[0]);
        }
        static void Main(string[] args)
        {
            string text = "hello";
            if (text.isCapital())// تم استدعاء الداله مع المتغير من نوع string
                Console.WriteLine("is capital letter");
            else
                Console.WriteLine("its not");
        }

```