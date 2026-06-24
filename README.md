<div dir="rtl" align="right">

# 🛒 LuxeCart Design System & E-Commerce Platform

An advanced, fully responsive E-commerce platform built as a graduation project. The application features a premium user interface, custom design system components, and smooth client-side interactions.

---

## 💡 فكرة المشروع (Project Concept)

تم بناء مشروع **LuxeCart** من الصفر باستخدام أحدث تقنيات الـ Frontend لضمان السرعة الفائقة والأداء المتميز في تصفح المنتجات وإدارة السلة وإتمام عمليات الشراء.
المنصة تركز بشكل أساسي على تقديم تجربة تسوق فاخرة وسلسة ومريحة للمستخدم لتواكب المواقع العالمية الفخمة **(Premium UX)**.

---

## 🎯 أهداف المشروع (Project Goals)

* **تجربة مستخدم فائقة (Premium UX):** تصميم واجهات تفاعلية جذابة وسهلة الاستخدام تناسب الهوية البصرية للمتاجر الفاخرة.
* **الأداء والسرعة الفائقة:** استغلال بيئة العمل الذكية لـ `Vite` لتقديم سرعة تحميل لحظية للمكونات والمنتجات.
* **التجاوب الكامل (Full Responsiveness):** دعم جميع الشاشات (موبايل، تابلت، شاشات مكتبية) بشكل مثالي وديناميكي باستخدام `Tailwind CSS`.

---

## 💎 الميزة التنافسية (Competitive Advantage)

* **Custom Design System:** تم بناء مكونات واجهة المستخدم مثل **Buttons, Cards, Modals** بشكل خاص ومستقل دون الاعتماد على مكتبات جاهزة تقليدية، مما يمنح التطبيق مرونة تامة في التعديل وأداءً فائق الخفة.
* **Advanced State Management:** إدارة تفاعلية متطورة للسلة **(Cart)** والمفضلة **(Favorites)** تضمن تحديث البيانات فورياً وبسلاسة أمام العميل دون أي تأخير أو إعادة تحميل للصفحة.

---
## 📸 Screenshots

<p align="center">
  <img src="./screenshots/screen1.png" alt="Screenshot 1" width="45%" />
  <img src="./screenshots/screen2.png" alt="Screenshot 2" width="45%" />
</p>

<p align="center">
  <img src="./screenshots/screen3.png" alt="Screenshot 3" width="45%" />
  <img src="./screenshots/screen4.png" alt="Screenshot 4" width="45%" />
</p>

<p align="center">
  <img src="./screenshots/screen5.png" alt="Screenshot 5" width="60%" />
</p>


## 🛠️ التقنيات المستخدمة (Tech Stack)

* **Frontend Library:** `React.js` + `TypeScript`
* **Build Tool:** `Vite`
* **Styling:** `Tailwind CSS`
* **Tools & Linters:** `ESLint`, `PostCSS`

---

## ✨ أهم مميزات المشروع (Key Features)

* 🛍️ **تصفح المنتجات:** عرض ذكي ومنظم للمنتجات مع إمكانية التصفية **(Filtering)**.
* 🛒 **نظام السلة المتطور:** إضافة وتعديل كميات المنتجات داخل السلة وحساب الإجمالي فورياً.
* ❤️ **قائمة المفضلة:** حفظ المنتجات للرجوع إليها لاحقاً برابط سريع وسلس.
* 🔐 **نظام المصادقة والتأمين (Authentication):** واجهات مخصصة لتسجيل الدخول وإنشاء الحساب لحماية بيانات العملاء **(Client-Side Simulation)**.
* 🌓 **الدعم اللوني التفاعلي:** هيكلية مهيأة ومستقرة لدعم الوضع الداكن والفاتح **(Dark / Light Mode)**.

---

## 📂 شرح مختصر لملفات المشروع (Project Structure)

* `public/` : الملفات الثابتة، الصور، والأيقونات الأساسية للموقع.
* `src/components/` : العناصر المشتركة القابلة لإعادة الاستخدام مثل الأزرار، الكروت، ومربعات الحوار.
* `src/hooks/` : الـ **Custom Hooks** لإدارة الحالات والمفضلة والسلة بشكل محلي وديناميكي مثل `useFavorites` و `useCart`.
* `src/pages/` : صفحات النظام الأساسية مثل `Home`, `Shop`, `Cart`, `Checkout`, `Product`, `Account`.
* `src/test/` : ملفات وإعدادات البيئة الاختبارية لضمان جودة الأكواد.
* `src/App.tsx` : المكون الرئيسي المسؤول عن التوجيه **Routing** بين الصفحات.
* `src/main.tsx` : نقطة انطلاق التطبيق وتحميل وإعداد ملفات الستايل الشاملة.

---

## 🚀 خطوات تشغيل المشروع محلياً (How to Run Locally)

لتشغيل المشروع على جهازك الشخصي، افتح الـ Terminal واكتب الأوامر التالية بالترتيب:

### 1) تثبيت المكتبات والاعتمادات الأساسية

```bash
npm install
```

### 2) تشغيل المشروع في بيئة التطوير المحلية

```bash
npm run dev
```

💡 سيظهر لك رابط محلي داخل الـ **Terminal** (مثل: `http://localhost:5173`)؛
قم بفتحه في المتصفح لاستعراض الموقع بشكل حي وتفاعلي.

---

## 🛑 التحديات التي قابلتنا أثناء التنفيذ (Challenges & Solutions)

### 1) تزامن البيانات المحلي (State Persistence)

واجهنا تحديًا في الحفاظ على المنتجات داخل السلة والمفضلة عند قيام المستخدم بعمل **Refresh** للصفحة.
قمنا بحل ذلك عبر بناء **Custom Hooks** تربط الـ **State** بالـ **LocalStorage** بشكل ديناميكي ومحمي، لضمان تجربة مستخدم مستقرة وسلسة.

### 2) تهيئة وإعداد بيئة TypeScript

في بداية الدمج واجهنا بعض التعارضات التقنية في الـ **Types** والموديلات الخاصة بالـ **Components**.
تم التغلب على ذلك بإعادة هيكلة ملفات `tsconfig.json` بدقة لضمان استقرار الأكواد وتجنب أخطاء وقت البناء **(Build-time Errors)**.

---

## 🔮 الأفكار والتطويرات المستقبلية (Future Work)

* **ربط بوابات الدفع الحقيقية:**
  دمج خدمات دفع عالمية ومحلية آمنة مثل **Stripe** و **Fawry** لتأمين عمليات الشراء الفعلية.

* **لوحة تحكم ذكية (Admin Dashboard):**
  بناء لوحة تحكم كاملة للمسؤولين لمتابعة الطلبات، المخزون، وتحليل المبيعات.

* **نظام التوصيات الذكي (AI Recommendations):**
  دمج خوارزميات ذكاء اصطناعي بسيطة لترشيح المنتجات للمستخدمين بناءً على سلوك التصفح الخاص بهم.

---

## 👥 أسماء أعضاء الفريق (Team Members)

* **Shahd Mansour Abdullah Abu Saada**
* **Basant Roshdy Gouda El-Shahat**
* **Rawan Mahmoud Hassan Ahmed**
* **Doaa Akram Shehab**

---

## 🎬 روابط الملحقات وتسليم المشروع (Project Links)

* 🔗 **رابط المستودع (GitHub Repository):**
  [اضغط هنا](https://github.com/ItcProjects-R4/SHR4_SWD2_S1_PROJECT2)

* 🌐 **رابط النسخة المباشرة (Live Demo):**
  [LuxeCart Store](https://luxe-cart-store.netlify.app)

* 🎥 **رابط فيديو الشرح الكامل:**
  *سيتم إضافة الرابط هنا فور تسجيل الفيديو.*

</div>


