# TBClassificaiton
Tuberculosis (TB) Chest X-ray Database
5)جمع بندی نهایی:
مجموعه داده حاضر از تصاویر ریه سالم و بیمار تشکیل شده است که دارای اطلاعات زیر است.

![image](https://user-images.githubusercontent.com/46417220/182558392-6b65d025-ffc3-4a68-af4f-e7969f2475a2.png)


که تعدادی از نمونه های آنرا می توان در تصویر زیر مشاهده کرد. 

![image](https://user-images.githubusercontent.com/46417220/182558509-02abb656-f7c8-451d-9d7e-2e72f50832f2.png)


برای فرایند آموزش مجموعه داده حاضر را به 3 دسته testing, validation, training با نسبت های 0.7, 0.2 و 0.1 تقسیم کردیم که به صورت زیر درآمده اند.

![image](https://user-images.githubusercontent.com/46417220/182558482-d6ec1091-7f33-4193-b2c4-78d9f8062296.png)



برای طبقه بندی تصاویر مجموعه داده حاضر از شبکه vgg16 با ساختار زیر استفاده کردیم.

![image](https://user-images.githubusercontent.com/46417220/182558541-c18f23f7-17c0-446e-93c8-f68eaacc16f6.png)



به دلیل عدم توازن داده ها از class weight استفاده کردیم که وزن هر کلاس به صورت زیر است.

![image](https://user-images.githubusercontent.com/46417220/182558578-becc53fb-1046-4ebf-ab34-0b02082d1db9.png)


فرایند آموزش با batch size=32 و epochs=20 روی مجموعه داده انجام شد که نتایج زیر حاصل شد.

نمودار loss/accuracy

![image](https://user-images.githubusercontent.com/46417220/182558615-7f4a79a2-7b94-42c2-aec9-c59759e5eb72.png)

نتایج precision، recall، f1-score

![image](https://user-images.githubusercontent.com/46417220/182558647-f16e15c0-167f-4661-b951-24467759f1ed.png)

نمودار ROC 


![image](https://user-images.githubusercontent.com/46417220/182558665-c185edd6-8577-423e-b5ec-969ba0533599.png)

نقشه حرارتی داده های آزمایشی


![image](https://user-images.githubusercontent.com/46417220/182558694-b1fd7f51-8d30-4335-804d-ca02dbb0ce54.png)

نمودار precision و recall و f1-score بر اساس threshold های مختلف بین 0 تا 1


![image](https://user-images.githubusercontent.com/46417220/182558719-32a2cf7e-8c27-4349-bc23-5045c42c84a8.png)

نمودار precision/recall


![image](https://user-images.githubusercontent.com/46417220/182558746-e6abf24c-beae-4ddd-9ba5-8e99409e1c51.png)

تصویر داده هایی که به غلط طبقه بندی شده اند.


![image](https://user-images.githubusercontent.com/46417220/182558770-81736bb2-1efc-49c0-877e-7d693a03ac17.png)
