# DL_project
پروژه نهایی درس یادگیری عمیق :

تشخیص اشیا و عمق آنها در فاصله ی مشخص در تصویر

*** توجه شود این قسمت به هیچ وجه جای گزین گزارش نمی شود و صرفا جهت دید کلی از پروژه و کدها است در نتیجه حتما فایل گزارش 
DL_project_report.pdf
قرار داده شده را مطالعه نمایید***

اعضای گروه:

علیرضا حشمتی 99206009

پیمان ناصری 96100522

توضیحات در مورد پروژه :

در این پروژه از دو تا شبکه ی جدا برای تشخیص اشیا و تخمین عمق آن ها استفاده شده است. که برای تشخیص اشیا از شبکه آماده ی
YOLO
کمک گرفته شده است و برای تخمین عمق، شبکه ای نزدیک به شبکه ی 
FastDepth
ارائه شده در مقاله به آدرس 
http://fastdepth.mit.edu/2019_icra_fastdepth.pdf 
استفاده شده است. از ویژگی های بارز هردو شبکه در کنار دقت خوبی که دارند، این است که سرعت شبکه ها در فاز اجرا بالا است. این موضوع کمک شایانی در تشکیل شبکه ی نهایی
برای تشخیص اشیا و عمق آن ها در فاصله ی معین می کند.

 پیاده سازی، و آموزش و ارزیابی شبکه ی تشخیص عمق در کد
 depth-estimation.ipynb 
 انجام شده است. از آنجا که شبکه ی معرفی شده از انکودر و دیکدر تشکیل شده است، در قسمت انکدر آن از شبکه ی آموزش دیده ی
 mobilenet
 استفاده شده است. که مقادیر پارامتر آن را از  ایجا
 https://drive.google.com/file/d/1MUlAe5L_qm0P0f5KGmmgHnA4GZDyOqkB/view?usp=sharing
 دانلود کنید و در کد ها استفاده کنید. 

کد 
DL_aplication_Project.ipynb 
برای تشکیل شبکه ی نهایی است و طوری نوشته شده است که به صورت کاربردی قابل استفاده باشد. در این کد هر دو شبکه ی تشخیص  اشیا و تخمین عمق به نحوی استفاده شده اند
که شبکه نهایی را تشکیل می دهند. برای اجرای این کد علاوه پارامتر های پیش آموزش شبکه ی 
mobilenet 
به بهترین مودل بدست آمده برای شبکه ی تخمین عمق در کد 
 depth-estimation.ipynb 
لازم است. می توانید کد اجرا نمایید و بهترین شبکه را بدست آورید و یا از لینک 
https://drive.google.com/file/d/1IzQ7tiAuDKLgoYG8-HCj8nnMVk_DBxOy/view?usp=sharing
بهترین مدل بدست آمده توسط ما را دریافت نمایید.

دقت شبکه ی
YOLO
با معیار 
0.579
mAP
است. معیار شبکه ی تخمین عمق با معیار دلتا 2
0.895
است که طبق معیار میانگینی که تعریف کردیم معیار شبکه ی نهایی 0.737 می شود.

آدرس دادگان 
NYU Depth Dataset V2
که در این پروژه استفاده شده است:
http://horatio.cs.nyu.edu/mit/silberman/nyu_depth_v2/nyu_depth_v2_labeled.mat

جزئیات همه نتایج، مباحث و تعاریف در گزارش 
DL_project_report.pdf
آمده است حتما معیار ارزیابی و مطالعه ی پروژه، گزارش قرار دهید.


