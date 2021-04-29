<div dir="rtl">

> params

هي كلمة تكتب مع معامل في الداله التي تستقبل المتغيرات ، تسمح باخذ قيم عددها غير محدود من انواع مختلفة اذا كانت من نوع اوبجكت او يمكن تحديد نوعها وتخزنها في مصفوفة

مثال :
<div>

```C#
public static void UseParams(params int[] list) // تستقبل متغيرات من نوع int وتخزنها في مصفوفه
    {
        for (int i = 0; i < list.Length; i++)
        {
            Console.Write(list[i] + " ");
        }
        Console.WriteLine();
    }

    public static void UseParams2(params object[] list)// // تستقبل متغيرات من نوع object وتخزنها في مصفوفه
    {
        for (int i = 0; i < list.Length; i++)
        {
            Console.Write(list[i] + " ");
        }
        Console.WriteLine();
    }
    ```