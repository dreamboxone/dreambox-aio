# Dreambox One / Two — Persian & Arabic Language Support

> **This image belongs to Dream Property GmbH.**
> The changes made to it are: Persian and Arabic language support was added,
> and the third-party GP4 / Gemini plugin suite was removed. enigma2 itself
> and the rest of the system are unmodified — nothing was unlocked or altered.

---

## فارسی

### این ایمیج چیست

ایمیج رسمی **Dreambox One** و **Dreambox Two** با افزودن پشتیبانی کامل از
زبان‌های راست‌به‌چپ.

### چه چیزی اضافه شده

- **پشتیبانی فارسی و عربی** — حروف به‌درستی به هم می‌چسبند و متن در جهت صحیح
  راست‌به‌چپ نمایش داده می‌شود: منوها، لیست کانال‌ها، EPG، تنظیمات، پیام‌ها،
  عنوان پنجره‌ها و صفحه‌های تنظیم تصویر.
- **اعداد فارسی** در جهت درست نمایش داده می‌شوند (۱۴۰۵ نه ۵۰۴۱)، که برای
  افزونه‌هایی مانند تقویم شمسی لازم است.
- **فونت فارسی** با پوشش کامل حروف پ، چ، ژ، ک، گ، ی و ارقام فارسی، روی همهٔ
  اسکین‌های همراه ایمیج.
- **۵۱۲ رشتهٔ ترجمه‌شدهٔ جدید فارسی** به‌همراه ۲۶ اصلاح واژگانی، و
  **۴۸۰ رشتهٔ ترجمه‌شدهٔ جدید عربی**. اولویت با منوی اصلی، درخت تنظیمات و
  صفحاتی است که کاربر بیشتر با آن‌ها سروکار دارد.

### چه چیزی حذف شده

بستهٔ افزونه‌های **GP4 / Gemini** به‌طور کامل حذف شده است: BluePanel،
Netcast، FileBrowser، AddonManager، QButton، StreamRipper، HwManager و بقیهٔ
اجزای آن، به‌همراه دو بستهٔ وابسته (`livestreamer` و `netcast-hoster`) که
بدون آن‌ها کار نمی‌کردند. مجموعاً ۱۸ بسته.

پایگاه‌دادهٔ بسته‌ها هم متناسب با آن پاک‌سازی شده، پس `apt` و `dpkg` وضعیت
سازگاری دارند و دنبال بسته‌ای که وجود ندارد نمی‌گردند.

کتابخانهٔ `youtube_dl` (بستهٔ `youtubegp`) عمداً نگه داشته شده — بستهٔ
مستقلی است که فقط پوشه‌اش را با GP4 شریک بود.

### نصب دستی پنل GP4.2 (اختیاری)

اگر بعداً پنل GP4.2 را خواستید، از داخل شل ریسیور (SSH یا تل‌نت) این را اجرا
کنید:

```
apt update && wget -O /tmp/geminilocale_all.deb http://download.blue-panel.com/geminilocale_gp42.php && apt install -y /tmp/geminilocale_all.deb
```

توجه: این دستور بسته را از سرور شخص ثالث می‌گیرد و بقیهٔ اجزای GP4 را هم به
دنبال خود نصب می‌کند.

### چه چیزی دست‌نخورده مانده

خودِ enigma2، درایورها، اسکین‌ها و بقیهٔ سیستم بدون تغییرند. جز حذف GP4،
تنها تفاوت‌ها با ایمیج اصلی، فایل‌های مربوط به زبان و فونت‌اند، به‌همراه
بسته‌های به‌روزرسانی‌شدهٔ خودِ سازندگان.

### فعال کردن زبان فارسی

ایمیج مانند گذشته با زبان انگلیسی بالا می‌آید:

**Menu → Setup → Language → Persian**

### نکته

پیام کوتاهی که هنگام «راه‌اندازی مجدد رابط گرافیکی» نمایش داده می‌شود، عمداً
به انگلیسی باقی مانده است. آن متن را خودِ هستهٔ برنامه در لحظهٔ خاموش شدن رسم
می‌کند، جایی که پشتیبانی راست‌به‌چپ در دسترس نیست؛ بنابراین انگلیسی ماندنش
درست‌تر از نمایش معکوس آن است.

### تشکر و اعتبار

این کار بدون زحمات این‌ها ممکن نبود:

- **Dream Property GmbH** — سازندهٔ Dreambox و نرم‌افزار enigma2
- **opendreambox** — سیستم‌عاملی که این ایمیج بر پایهٔ آن ساخته شده
- **[i-have-a-dreambox.com](https://i-have-a-dreambox.com/)** — جامعه‌ای که
  دانش و پشتیبانی این دستگاه‌ها را زنده نگه داشته است

تمام حقوق enigma2 و ایمیج پایه متعلق به Dream Property GmbH است.

---

## English

### What this is

The official **Dreambox One** and **Dreambox Two** image, with full
right-to-left language support added.

### What was added

- **Persian and Arabic support** — letters join correctly and text reads in
  proper right-to-left order throughout: menus, channel list, EPG, settings,
  message dialogs, window titles and the picture-tuning screens.
- **Persian digits** now read in the correct direction (۱۴۰۵, not ۵۰۴۱),
  which plugins such as the Jalali calendar depend on.
- **A Persian-capable font** covering پ, چ, ژ, ک, گ, ی and Persian digits,
  applied to every skin shipped with the image.
- **512 newly translated Persian strings** plus 26 wording corrections, and
  **480 newly translated Arabic strings**. Priority was given to the main
  menu, the setup tree and the screens users actually open.

### What was removed

The **GP4 / Gemini** plugin suite has been removed in full: BluePanel,
Netcast, FileBrowser, AddonManager, QButton, StreamRipper, HwManager and the
rest of its components, along with two packages that depended on it and could
not work without it (`livestreamer` and `netcast-hoster`). Eighteen packages
in total.

The package database was cleaned up to match, so `apt` and `dpkg` stay
consistent rather than looking for packages that are no longer there.

The `youtube_dl` library (package `youtubegp`) was deliberately kept — it is
an independent package that merely shared a directory with GP4.

### Installing the GP4.2 panel manually (optional)

If you want the GP4.2 panel back later, run this from a shell on the receiver
(SSH or telnet):

```
apt update && wget -O /tmp/geminilocale_all.deb http://download.blue-panel.com/geminilocale_gp42.php && apt install -y /tmp/geminilocale_all.deb
```

Note that this fetches the package from a third-party server and pulls in the
rest of the GP4 components with it.

### What was left alone

enigma2 itself, the drivers, the skins and the rest of the system are
untouched. Apart from the GP4 removal, the only differences from the original
image are the language and font files, together with the maintainers' own
updated packages.

### Enabling Persian

The image still starts in English:

**Menu → Setup → Language → Persian**

### A note

The brief message shown while the GUI restarts is deliberately left in
English. That text is drawn by the application core as it shuts down, past
the point where right-to-left support is available, so English is a better
result than showing it reversed.

### Credits and thanks

This work would not exist without:

- **Dream Property GmbH** — makers of the Dreambox and of enigma2
- **opendreambox** — the operating system this image is built on
- **[i-have-a-dreambox.com](https://i-have-a-dreambox.com/)** — the community
  that keeps the knowledge and support for these receivers alive

All rights to enigma2 and to the base image remain with Dream Property GmbH.

---

## العربية

### ما هذه النسخة

نسخة **Dreambox One** و **Dreambox Two** الرسمية، مع إضافة دعم كامل للغات
التي تُكتب من اليمين إلى اليسار.

### ما الذي أُضيف

- **دعم اللغتين العربية والفارسية** — تتصل الحروف ببعضها بشكل صحيح ويُعرض
  النص في اتجاهه الصحيح من اليمين إلى اليسار: القوائم وقائمة القنوات ودليل
  البرامج والإعدادات ورسائل النظام وعناوين النوافذ وشاشات ضبط الصورة.
- **الأرقام الفارسية** تُعرض في اتجاهها الصحيح (۱۴۰۵ وليس ۵۰۴۱)، وهو ما
  تحتاجه إضافات مثل التقويم الشمسي.
- **خط يدعم الحروف الفارسية** بما فيها پ و چ و ژ و ک و گ و ی والأرقام
  الفارسية، مُطبَّق على كل الأشكال المرفقة بالنسخة.
- **٤٨٠ نصًّا مترجمًا جديدًا إلى العربية**، إضافة إلى ٥١٢ نصًّا إلى الفارسية.
  أُعطيت الأولوية للقائمة الرئيسية وشجرة الإعدادات والشاشات التي يستخدمها
  المستخدم فعليًّا.

### ما الذي أُزيل

أُزيلت حزمة إضافات **GP4 / Gemini** بالكامل: BluePanel و Netcast و
FileBrowser و AddonManager و QButton و StreamRipper و HwManager وبقية
مكوّناتها، إضافة إلى حزمتين كانتا تعتمدان عليها ولا تعملان بدونها
(`livestreamer` و `netcast-hoster`). ثماني عشرة حزمة إجمالًا.

نُظّفت قاعدة بيانات الحزم بما يوافق ذلك، فيبقى `apt` و `dpkg` متّسقَين بدل
البحث عن حزم لم تعد موجودة.

أُبقيت مكتبة `youtube_dl` (حزمة `youtubegp`) عن قصد، فهي حزمة مستقلة كانت
تشارك GP4 المجلد نفسه فقط.

### تثبيت لوحة GP4.2 يدويًّا (اختياري)

إن أردت لوحة GP4.2 لاحقًا، نفّذ هذا الأمر من سطر أوامر الجهاز (عبر SSH أو
telnet):

```
apt update && wget -O /tmp/geminilocale_all.deb http://download.blue-panel.com/geminilocale_gp42.php && apt install -y /tmp/geminilocale_all.deb
```

لاحظ أن هذا الأمر يجلب الحزمة من خادم طرف ثالث ويجرّ معه بقية مكوّنات GP4.

### ما الذي لم يتغيّر

برنامج enigma2 نفسه والمشغّلات والأشكال وبقية النظام لم تُمسّ. وبخلاف إزالة
GP4، فإن الفروق الوحيدة عن النسخة الأصلية هي ملفات اللغة والخطوط، إضافة إلى
حزم التحديث الصادرة عن القائمين على النسخة أنفسهم.

### تفعيل اللغة

تبدأ النسخة باللغة الإنجليزية كما كانت:

**Menu → Setup → Language**

### ملاحظة

الرسالة القصيرة التي تظهر أثناء إعادة تشغيل الواجهة تُركت بالإنجليزية عن قصد.
فهذا النص يرسمه قلب البرنامج لحظة الإغلاق، بعد أن يصبح دعم الكتابة من اليمين
إلى اليسار غير متاح، ولذلك فإن بقاءه بالإنجليزية أفضل من عرضه معكوسًا.

### الشكر والتقدير

لم يكن هذا العمل ممكنًا لولا:

- **Dream Property GmbH** — صانعة أجهزة Dreambox وبرنامج enigma2
- **opendreambox** — نظام التشغيل الذي بُنيت عليه هذه النسخة
- **[i-have-a-dreambox.com](https://i-have-a-dreambox.com/)** — المجتمع الذي
  يحافظ على المعرفة والدعم الخاص بهذه الأجهزة

جميع الحقوق الخاصة ببرنامج enigma2 وبالنسخة الأساسية محفوظة لشركة
Dream Property GmbH.
