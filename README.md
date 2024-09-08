# بسم الله الرحمن الرحيم

## Login Page

## المشروع من تصميم (محمد القاضي)

هذا مشروع Flutter لعملية تسجيل الدخول والتسجيل للمستخدمين، باستخدام Firebase كخدمة خلفية. البرنامج بيقدم 3 طرق للتسجيل:

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

لتشغيل البرنامج محليًا، اتبع الخطوات التالية:

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

   بعد نسخ المشروع، انتقل إلى مجلد المشروع:

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

### إعداد Firebase CLI

لتشغيل التطبيق بشكل صحيح، يجب عليك تشغيل Firebase CLI أولاً وتثبيت Firebase في مشروعك باستخدام الأوامر التالية:

```bash
dart pub global activate flutterfire_cli
flutterfire configure
```

### إعداد تطبيق فيسبوك

يجب عليك إنشاء تطبيق جديد كـ Consumer في Meta for Developers، ثم إعداد التطبيق في ملف `AndroidManifest.xml` بإضافة الكود التالي:

```xml
<meta-data android:name="com.facebook.sdk.ApplicationId"
            android:value="@string/facebook_app_id" />
<meta-data android:name="com.facebook.sdk.ClientToken"
            android:value="@string/facebook_client_token" />
<activity android:name="com.facebook.FacebookActivity"
          android:configChanges="keyboard|keyboardHidden|screenLayout|screenSize|orientation"
          android:label="@string/app_name" />
<activity android:name="com.facebook.CustomTabActivity" android:exported="true">
    <intent-filter>
        <action android:name="android.intent.action.VIEW" />
        <category android:name="android.intent.category.DEFAULT" />
        <category android:name="android.intent.category.BROWSABLE" />
        <data android:scheme="@string/fb_login_protocol_scheme" />
    </intent-filter>
</activity>
```

أضف أيضًا الملف التالي داخل مجلد `res/values` كملف `strings.xml`:

```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <string name="app_name">test</string>
    <string name="facebook_app_id">Placeholder for Facebook App ID</string>
    <string name="fb_login_protocol_scheme">Placeholder for FB Login Protocol Scheme</string>
    <string name="facebook_client_token">Placeholder for Facebook Client Token</string>
    <string name="default_notification_channel_id" translatable="false">fcm_default_channel</string>
</resources>
```

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

<p align="center" class="grid">
  <img src="https://github.com/kady-x/login_page/blob/main/assets/screens/1.jpeg" alt="واجهة المستخدم الرئيسية" width="200"/>
  <img src="https://github.com/kady-x/login_page/blob/main/assets/screens/2.jpeg" alt="تسجيل الدخول" width="200"/>
  <img src="https://github.com/kady-x/login_page/blob/main/assets/screens/3.jpeg" alt="تسجيل حساب جديد" width="200"/>
  <img src="https://github.com/kady-x/login_page/blob/main/assets/screens/4.jpeg" alt="قائمة الدول" width="200"/>
  <img src="https://github.com/kady-x/login_page/blob/main/assets/screens/5.jpeg" alt="واجهة التحقق من صلاحية الإيميل" width="200"/>
  <img src="https://github.com/kady-x/login_page/blob/main/assets/screens/6.jpeg" alt="واجهة التحقق من الإيميل" width="200"/>
  <img src="https://github.com/kady-x/login_page/blob/main/assets/screens/7.jpeg" alt="واجهة إعداد كلمة السر" width="200"/>
  <img src="https://github.com/kady-x/login_page/blob/main/assets/screens/8.jpeg" alt="واجهة المستخدم الرئيسية للحساب" width="200"/>
  <img src="https://github.com/kady-x/login_page/blob/main/assets/screens/9.jpeg" alt="واجهة المستخدم الرئيسية لمستخدمي جوجل وفيس بوك" width="200"/>
</p>

## تحميل التطبيق

يمكنك العثور على أو تحميل النسخة المدعومة من التطبيق (APK) من الرابط التالي:

- [تحميل التطبيق](https://github.com/kady-x/login_page/blob/main/apk/app-release.apk)

---

## أهمية المشروع

هذا المشروع مهم للغاية بالنسبة لي، حيث يساعدني على تحسين مهاراتي في تطوير التطبيقات وتعلم تقنيات جديدة. إذا كان لديك أي ملاحظات أو اقتراحات لتحسين المشروع، سأكون سعيدًا جدًا بمساعدتك! 🌟
