# TBClassificaiton
Tuberculosis (TB) Chest X-ray Database
5)جمع بندی نهایی:
مجموعه داده حاضر از تصاویر ریه سالم و بیمار تشکیل شده است که دارای اطلاعات زیر است.

![image](/uploads/ce5abce77569451ff321462aa0ae6da4/image.png)


که تعدادی از نمونه های آنرا می توان در تصویر زیر مشاهده کرد. 

![image](/uploads/3c075802668e08caf065a8981167d1af/image.png)


برای فرایند آموزش مجموعه داده حاضر را به 3 دسته testing, validation, training با نسبت های 0.7, 0.2 و 0.1 تقسیم کردیم که به صورت زیر درآمده اند.

![image](/uploads/6de505375ac63c927ca96a2c6d402757/image.png)



برای طبقه بندی تصاویر مجموعه داده حاضر از شبکه vgg16 با ساختار زیر استفاده کردیم.

![image](/uploads/e60431206099d29ed361586ff3c023bb/image.png)



به دلیل عدم توازن داده ها از class weight استفاده کردیم که وزن هر کلاس به صورت زیر است.

![image](/uploads/a196157ff7f709f213f799d99e5fa2e5/image.png)


فرایند آموزش با batch size=32 و epochs=20 روی مجموعه داده انجام شد که نتایج زیر حاصل شد.

نمودار loss/accuracy

![image](/uploads/4ae288d45dac25f3b77554a99c2d9c85/image.png)

نتایج precision، recall، f1-score

![image](/uploads/66076a211ad047c71444052d5ad367e4/image.png)

نمودار ROC 


![image](/uploads/3a66f4156a995574371f8a6330482e76/image.png)

نقشه حرارتی داده های آزمایشی


![image](/uploads/05b440ce4e48da30ac3ab76a4bf8d009/image.png)

نمودار precision و recall و f1-score بر اساس threshold های مختلف بین 0 تا 1


![image](/uploads/60bf399c397cfe4ba6afb2f32a5554b5/image.png)

نمودار precision/recall


![image](/uploads/e6ba98f7e201b9fb4b274ad55717c1c4/image.png)

تصویر داده هایی که به غلط طبقه بندی شده اند.


![image](/uploads/6127838673db932a3effef79014db65b/image.png)
