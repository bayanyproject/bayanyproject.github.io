---
layout: post
title: تنصيب منصة آر
category: "learn r"
description: تُتبر منصة آر من أقوى الأدوات البرمجية لتحليل البيانات وإجراء العمليات الإحصائية، وهي متوفرة للتنصيب بسهولة على معظم أنظمة التشغيل. في هذا الملف سنوضح كيفية تنصيب آر على ويندوز، أجهزة الماك، وكذا نظام اللينكس، بالإضافة إلى الخيارات السحابية.
img: <img src="https://raw.githubusercontent.com/bayanyproject/bayanyproject.github.io/refs/heads/main/images/R_logo.png" width='100' height= auto/>
---
تجدون هنا بعض المعلومات الموجزة عن كيفية تنصيب منصة آر على مختلف أنظمة التشغيل الحاسوبية. شخصيا ، أعمل على منصة **Debian** وهو من أشهر أنظمة **لينكس** كما سبق لي و أن نصبت آر على أجهزة **الويندوز** و لكن رغم ذلك ستجدون بعض النصائح و الروابط الخاصة بتنصيب المنصة على أغلب الوسائط. بالرغم من كل هذا ، فهذه النصائح قد لا تكون مناسبة لكل الأجهزة و قد تحمل معلومات غير محينة بالنسبة لمختلف إصدارات أنظمة التشغيل أو إصدارات آر و لذا فيرجى التعامل معها بشيء من الحيطة. 

تُعتبر منصة **R** من أقوى الأدوات البرمجية لتحليل البيانات وإجراء العمليات الإحصائية، وهي متوفرة للتنصيب بسهولة على معظم أنظمة التشغيل. ستجد أسفله بعض المعلومات حول كيفية تنصيب R على **Windows**، **macOS**، و**Linux** بالإضافة إلى بعض الخيارات السحابية مثل [آر ستوديو كلاود RStudio Cloud](https://posit.cloud).

أغلب خيارات التنصيب موجودة على [الموقع الرسمي لتحميل برنامج آر](https://cran.r-project.org) (https://cran.r-project.org) و المسمى [كران CRAN](https://cran.r-project.org) والتي هي أولى حروف كلمات The Comprehensive R Archive Network أو الشبكة الشاملة لأرشيف آر و التي تحوي شبكة موارد توزيع البرنامج و أحزمته المختلفة على الانترنت أو ftp عبر العالم. يتم التنصيب عادة بعد اختيار أحد مصادر مستودعات البرنامج و التي ينصح أن تكون الأقرب جغرافيا.

![الموقع الرسمي لتحميل برنامج آر](/images/R/rinstall1.png "الموقع الرسمي لتحميل برنامج آر")

---

## 1. تنصيب R على Windows

للبدء باستخدام R على نظام Windows يفضل تنزيل ملف التنصيب مباشرة ثم تشغيله. 
1. **تنزيل البرنامج**:  
   ينزل الملف الخاص بالتنصيب من [الموقع الرسمي لـ R](https://cran.r-project.org)، بعد الولوج ، اختر "Download R for Windows".
   
   ![تنصيب آر على ويندوز](/images/R/rinstallwin2.png "تنصيب آر على ويندوز")
   
   عدة اختيارات لملف التنصيب ستتاح في النافذة المقبلة. بالنسبة لأكثر المستعملين و خاصة إن كنت تنصبه لأول مرة ، اختر الملف الموجود على base.
   
   ![تنصيب آر على ويندوز](/images/R/rinstallwin3.png "تنصيب آر على ويندوز")

2. **التثبيت**:  
   شغّل الملف التنفيذي الذي تم تنزيله (.exe)، واتبع الإرشادات خطوة بخطوة. يُمكنك ترك الإعدادات الافتراضية أو تخصيصها حسب احتياجاتك.  
3. **التأكد من التثبيت**:  
   بعد انتهاء العملية، افتح **R GUI** أو **Command Prompt** واكتب الأمر التالي:  
   ```R
   version
   ```  
   سيظهر لك الإصدار المثبت من R.

## 2. تنصيب R على macOS
للمستخدمين الذين يعملون على أنظمة macOS:  
1. **تحميل ملف التثبيت**: انتقل إلى [الموقع الرسمي لـ R](https://cran.r-project.org)، واختر macOS، ثم حمل الإصدار الملائم لنوع جهازك، arm64 أو x86-64bit.

   ![تنصيب آر على أجهزة ماك](/images/R/rinstallmac4.png "تنصيب آر على أجهزة ماك")
   
2. **التثبيت**: افتح ملف التثبيت (.pkg) واتبع الخطوات التلقائية. يتم تثبيت R تلقائيًا ضمن المجلد `/Applications`.  
3. **التأكد من التشغيل**: افتح **Terminal** واكتب:  
   ```
   R
   ```  
   إذا ظهرت واجهة R النصية، فهذا يعني أن التثبيت تم بنجاح.

## 3. تنصيب R على Linux
لتثبيت R على أنظمة لينكس المختلفة:  
1. **إضافة المستودعات وتحديثها**: افتح الطرفية (Terminal) وأدخل الأوامر المناسبة لتوزيعتك. على سبيل المثال:  
   - **Ubuntu/Debian**:  
     ```
     sudo apt update
     sudo apt install r-base
     ```  
   - **Fedora/CentOS**:  
     ```
     sudo dnf install R
     ```  
2. **التأكد من التثبيت**: اكتب `R` في الطرفية أو **Terminal**. إذا ظهرت الواجهة النصية لـ R، فكل شيء جاهز.

كما يمكن تثبيت حزمة مكتملة منزلة من الموقع بغرض الحصول على أحدث نسخة و هو الأمر الذي قد يستلزم بعض الإعداد بالنظر إلى إصدار نظام تشغيل اللينكس الخاص بك. الطريقة المبينة أعلاه باعتماد مستوعات أنظمة اللينكس الرسمية و المبينة أعلاه هنا تبقى دائما أسهل.

## 4. استخدام R على السحابة
إذا كنت تفضل العمل بدون تثبيت محلي، يمكنك استخدام R على السحابة cloud  و ذلك باستعمال معالج Rstudio:  
- **RStudio Cloud**: منصة توفر بيئة تطوير متكاملة تعمل عبر المتصفح. يمكنك التسجيل مجانًا على [RStudio Cloud](https://posit.cloud).  
- **Google Colab**: يدعم Google Colab لغة R باستخدام إضافة `rpy2`.  

## 5. الأجهزة المحمولة
بالرغم من أن R غير متاح رسميًا للأجهزة المحمولة، يمكن تشغيله باستخدام تطبيقات مثل **Termux** على Android، أو استخدام أدوات السحابة عبر المتصفح.

## 6. تثبيت أحد المعالجات مثل RStudio أو RKward (اختياري) :
قد يستلزم العمل اليومي على R استعمال معالج للشفرة بدل الكتابة مباشرة على الطرفية و لذا توجد معالجات جيدة تتعامل مع آر و أكثرها شيوعا هو Rstudio. سنتناول هاته المعالجات في مقال آخر.
