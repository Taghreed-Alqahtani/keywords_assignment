<div dir="rtl">

> break

تستعمل للخروج من الجمل التكرارية وأيضا من switch عند حدوث شرط 

مثال :

int i = 0;
while (i < 10) 
{
  Console.WriteLine(i);
  i++;
  if (i == 4) 
  {
    break;// اذا اصبحت قيمة i تساوي صفر تخرج ويتوقف التكرار
  }
}

<div>