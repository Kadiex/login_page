# بسم الله الرحمن الرحيم

## Login Page

## المشروع ده من تصميم (محمد القاضي)

ده مشروع Flutter لعملية تسجيل الدخول والتسجيل للمستخدمين، واستخدمت Firebase كخدمة خلفية. البرنامج بيقدم 3 طرق للتسجيل:

- إنشاء حساب جديد.
- الدخول بحساب جوجل.
- الدخول بحساب فيسبوك.

![Flutter](https://img.shields.io/badge/Flutter-v3.5.1-blue)
![Firebase](https://img.shields.io/badge/Firebase-v9.0.0-orange)

## المحتويات

- [المميزات](#المميزات)
- [البدء](#البدء)
- [التثبيت](#التثبيت)
- [الاستخدام](#الاستخدام)
- [إعداد Firebase](#إعداد-firebase)
- [الاعتماديات](#الاعتماديات)
- [المساهمة](#المساهمة)
- [الرخصة](#الرخصة)
- [لقطات الشاشة](#لقطات-الشاشة)

## المميزات

- واجهات مستخدم سهلة الاستخدام لتسجيل الدخول والتسجيل.
- نظام Firebase Authentication لتأمين عمليات الدخول والخروج.
- التحقق من صحة بيانات المدخلات.
- تصميم مستجيب باستخدام Widgets في Flutter.
- استخدام الرسوم المتحركة باستخدام Lottie.
- مكونات واجهة مستخدم حديثة مع Shimmer و Cupertino icons.

## البدء

علشان تشغل البرنامج محليًا، اتبع الخطوات دي.

## المتطلبات المبدئية

- Flutter SDK (الإصدار 3.5.1)
- Dart SDK
- حساب على Firebase
- Android Studio أو Visual Studio Code

## التثبيت

1. **نسخ المستودع:**

   ```bash
   git clone https://github.com/kady-x/login_page.git
   ```

2. **تثبيت الاعتماديات:**

   بعد ما تنسخ المشروع، انتقل إلى مجلد المشروع:

   ```bash
   cd login_page
   ```

   ثم شغل الأمر التالي لتثبيت الاعتماديات:
   flutter pub get

   تشغيل التطبيق:
   بعد تثبيت الاعتماديات، شغل التطبيق عن طريق:
   flutter run

## الاستخدام

### نظام المصادقة (Auth)

1. إنشاء حساب جديد:
   🔐 افتح التطبيق واختر "إنشاء حساب جديد".
   📝 أدخل بياناتك مثل الاسم، البريد الإلكتروني، وكلمة المرور.
   ✅ اضغط على زر "تسجيل" لإنشاء الحساب.

2. الدخول بحساب جوجل:

   ☁️ افتح التطبيق واختر "تسجيل الدخول بحساب جوجل".
   📧 اختر حساب جوجل المطلوب من قائمة الحسابات المتاحة.
   ➡️ سيتم توجيهك إلى صفحة التطبيق بعد تسجيل الدخول بنجاح.

3. الدخول بحساب فيسبوك:

   📘 افتح التطبيق واختر "تسجيل الدخول بحساب فيسبوك".
   🔑 أدخل بيانات حسابك على فيسبوك إذا لزم الأمر.
   🎉 بعد نجاح العملية، ستحصل على إمكانية الدخول إلى التطبيق.

## إعداد Firebase

   1- قم بإنشاء مشروع جديد على Firebase Console.
   2- اتبع التعليمات لإعداد Firebase Authentication.
   3- أضف بيانات اعتماد Google و Facebook في إعدادات المصادقة.
   4- احصل على ملف google-services.json و GoogleService-Info.plist وقم بإضافتهم إلى المشروع.

## الاعتماديات

  ```bash
  cupertino_icons: ^1.0.8
  get: ^4.6.6
  http: ^1.2.2
  lottie: ^3.1.2
  dartz: ^0.10.1
  shared_preferences: ^2.3.2
  firebase_core: ^3.3.0
  firebase_core_platform_interface: ^5.2.0
  firebase_auth: ^5.1.4
  google_sign_in: ^6.2.1
  flutter_facebook_auth: ^7.0.1
  path: ^1.9.0
  image_picker: ^1.1.2
  image_cropper: ^8.0.2
  flutter_customs: ^0.0.28
  otp_text_field: ^1.1.3
  cached_network_image: ^3.4.0
  ```

## المساهمة

أهلا وسهلا بأي مساهمات! لو عندك أي اقتراحات أو تعديلات، لا تتردد في فتح قضية على GitHub.

## الرخصة

هذا المشروع مرخص بموجب رخصة MIT، يمكنك استخدامه كما تشاء.

## لقطات الشاشة

<p align="center" class="scroll" >
     <img width="200px" src="https://github.com/kady-x/login_page/blob/main/assets/screens/1.jpeg" alt="App screen shot">
     &nbsp;&nbsp;&nbsp;
     <img width="200px" src="https://github.com/kady-x/login_page/blob/main/assets/screens/2.jpeg" alt="App screen shot">
     &nbsp;&nbsp;&nbsp;
     <img width="200px" src="https://github.com/kady-x/login_page/blob/main/assets/screens/3.jpeg" alt="App screen shot">
     &nbsp;&nbsp;&nbsp;
     <img width="200px" src="https://github.com/kady-x/login_page/blob/main/assets/screens/4.jpeg" alt="App screen shot">
     &nbsp;&nbsp;&nbsp;
     <img width="200px" src="https://github.com/kady-x/login_page/blob/main/assets/screens/5.jpeg" alt="App screen shot">
     &nbsp;&nbsp;&nbsp;
     <img width="200px" src="https://github.com/kady-x/login_page/blob/main/assets/screens/6.jpeg" alt="App screen shot">
     &nbsp;&nbsp;&nbsp;
     <img width="200px" src="https://github.com/kady-x/login_page/blob/main/assets/screens/7.jpeg" alt="App screen shot">
     &nbsp;&nbsp;&nbsp;
     <img width="200px" src="https://github.com/kady-x/login_page/blob/main/assets/screens/8.jpeg" alt="App screen shot">
     &nbsp;&nbsp;&nbsp;
     <img width="200px" src="https://github.com/kady-x/login_page/blob/main/assets/screens/9.jpeg" alt="App screen shot">
     &nbsp;&nbsp;&nbsp;
</p>

إذا كنت بحاجة إلى مزيد من التفاصيل أو التعديلات، فلا تتردد في إخباري! 🌟
