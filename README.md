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
- [تحميل التطبيق](#تحميل-التطبيق)

## المميزات

- واجهات مستخدم سهلة الاستخدام لتسجيل الدخول والتسجيل.
- نظام Firebase Authentication لتأمين عمليات الدخول والخروج.
- التحقق من صحة بيانات المدخلات.
- تصميم مستجيب باستخدام Widgets في Flutter.
- استخدام الرسوم المتحركة باستخدام Lottie.
- مكونات واجهة مستخدم حديثة مع Shimmer و Cupertino icons.

## البدء

علشان تشغل البرنامج محليًا، اتبع الخطوات دي.

### المتطلبات المبدئية

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

   ```bash
   flutter pub get
   ```

   لتشغيل التطبيق:

   ```bash
   flutter run
   ```

## الاستخدام

### نظام المصادقة (Auth)

1. **إنشاء حساب جديد:**
   🔐 افتح التطبيق واختر "إنشاء حساب جديد".  
   📝 أدخل بياناتك مثل الاسم، البريد الإلكتروني، وكلمة المرور.  
   ✅ اضغط على زر "تسجيل" لإنشاء الحساب.  

2. **الدخول بحساب جوجل:**
   ☁️ افتح التطبيق واختر "تسجيل الدخول بحساب جوجل".  
   📧 اختر حساب جوجل المطلوب من القائمة.  
   ➡️ سيتم توجيهك إلى صفحة التطبيق بعد تسجيل الدخول بنجاح.  

3. **الدخول بحساب فيسبوك:**
   📘 افتح التطبيق واختر "تسجيل الدخول بحساب فيسبوك".  
   🔑 أدخل بيانات حسابك على فيسبوك إذا لزم الأمر.  
   🎉 بعد نجاح العملية، ستحصل على إمكانية الدخول إلى التطبيق.  

## إعداد Firebase

1. قم بإنشاء مشروع جديد على Firebase Console.
2. اتبع التعليمات لإعداد Firebase Authentication.
3. أضف بيانات اعتماد Google و Facebook في إعدادات المصادقة.
4. احصل على ملفات `google-services.json` و `GoogleService-Info.plist` وأضفهم إلى المشروع.

## الاعتماديات

```bash
cupertino_icons: ^1.0.8
get: ^4.6.6
http: ^1.2.2
lottie: ^3.1.2
dartz: ^0.10.1
shared_preferences: ^2.3.2
firebase_core: ^3.3.0
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

### واجهة المستخدم الرئيسية

<img src="https://github.com/kady-x/login_page/blob/main/assets/screens/1.jpeg" alt="واجهة المستخدم الرئيسية" width="200"/>

---

### واجهة تسجيل الدخول

<img src="https://github.com/kady-x/login_page/blob/main/assets/screens/2.jpeg" alt="تسجيل الدخول" width="200"/>

---

### واجهة تسجيل حساب جديد

<img src="https://github.com/kady-x/login_page/blob/main/assets/screens/3.jpeg" alt="تسجيل حساب جديد" width="200"/>

---

### قائمة الدول

<img src="https://github.com/kady-x/login_page/blob/main/assets/screens/4.jpeg" alt="قائمة الدول" width="200"/>

---

### واجهة التحقق من صلاحية الإيميل

<img src="https://github.com/kady-x/login_page/blob/main/assets/screens/5.jpeg" alt="واجهة التحقق من صلاحية الإيميل" width="200"/>

---

### واجهة التحقق من الإيميل

<img src="https://github.com/kady-x/login_page/blob/main/assets/screens/6.jpeg" alt="واجهة التحقق من الإيميل" width="200"/>

---

### واجهة إعداد كلمة السر

<img src="https://github.com/kady-x/login_page/blob/main/assets/screens/7.jpeg" alt="واجهة إعداد كلمة السر" width="200"/>

---

### واجهة المستخدم الرئيسية للحساب

<img src="https://github.com/kady-x/login_page/blob/main/assets/screens/8.jpeg" alt="واجهة المستخدم الرئيسية للحساب" width="200"/>

---

### واجهة المستخدم الرئيسية لمستخدمي جوجل وفيس بوك

<img src="https://github.com/kady-x/login_page/blob/main/assets/screens/9.jpeg" alt="واجهة المستخدم الرئيسية لمستخدمي جوجل وفيس بوك" width="200"/>

---

## تحميل التطبيق

يمكنك العثور على أو تحميل النسخة المدعومة من التطبيق (APK) من الرابط التالي:

- [تحميل التطبيق](https://github.com/kady-x/login_page/blob/main/apk/app-release.apk)

---

## أهمية المشروع

أنا كنت مهتم جدًا بالمشروع ده، وركزت على تطبيق مبادئ SOLID في الكود بتاعي. الهدف كان إن المشروع يساعدني على تحسين مستوايا في تطوير التطبيقات وتعلّم تقنيات جديدة. المشروع ده مهم بالنسبة لي عشان بيعد نقطة انطلاق لتنمية مهاراتي في البرمجة. لو عندك أي ملاحظات أو اقتراحات لتحسين المشروع، أكون سعيد جدًا بمساعدتك! 🌟
