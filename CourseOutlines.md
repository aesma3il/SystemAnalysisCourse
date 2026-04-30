# Systems Analysis - Complete Course Topics

## 1. Introduction & Personal Journey
- About Me
- How I Turned the Challenge of Understanding Systems Analysis into a Skill I Enjoy and Practice

## 2. Real-World Experience
- First Job Interview in Systems Analysis
- What Questions Were Asked
- What Was Required (Projects)
- The Test / Practical Assignment

## 3. How to Study This Course
- How to Approach These Lectures
- Learning Strategy for Maximum Benefit

## 4. Tools & Preparation
- Tools You Will Need During the Course
- Software and Resources


## 6. Fundamental Concepts Refresher
- What is a Computer?
- Input → Process → Output → Storage

## 7. Business & Data Concepts
- What is a Business?
- Data vs Information vs Knowledge vs Wisdom

## 8. Systems Thinking
- What is a System?
- Components of a System

## 9. Information Systems
- Introduction to Information Systems
- **Definition:** A set of interrelated components that collect, process, store, and provide information to support business tasks
- Key Characteristics:
  - Includes people, processes, and technology
  - Transforms data → information → knowledge

## 10. Components of Information Systems
- People
- Processes
- Data
- Technology

## 11. System Analyst Role
- Responsibilities of a System Analyst
- Skills Required
- Role in bridging business and technology

## 12. System Development Life Cycle (SDLC)
### Project Phases:
- **Planning** → Why build the system?
- **Analysis** → Who, What, When, Where?
- **Design** → How will the system work?
- **Implementation** → System delivery and deployment


# دراسة حالة: منصة فهد للتأجير - النظام الوسيط بين المؤجر والمستأجر

## نظرة عامة

فهد يعمل كوسيط نشيط يربط بين ملاك الأصول (مثل الشقق، السيارات، والأراضي) وبين الأشخاص الذين يرغبون في استئجار هذه الأصول. يعتمد في عمله على شبكة علاقات واسعة بناها مع الملاك والمستفيدين، حيث يقدم خدمة تنظيم وتأمين عملية التأجير مقابل مبلغ مالي بسيط يمثل عمولة على الخدمة.

مع توسع نشاطه وتعدد العمليات التي يديرها بشكل يدوي، أصبح من الضروري وجود نظام متكامل ينظم هذه العلاقة ويضبط جميع الإجراءات بشكل واضح وموثوق.

## طلب تطوير المنصة

توجه فهد إلى المهندس عبدالله إسماعيل وطلب منه تطوير منصة إلكترونية تكون وسيطًا رقميًا بين المؤجر والمستأجر، بحيث تقوم المنصة بتنظيم العملية بالكامل:
- عرض الأصول
- إتمام التعاقد
- إدارة الدفع
- أخذ عمولة بعد كل عملية تأجير ناجحة

## أهداف النظام

النظام يمثل منصة وسيطة هدفها الأساسي:
- تنظيم العلاقة بين المؤجر والمستأجر
- تسهيل إجراءات التعاقد والدفع
- ضمان حقوق الطرفين

---

## سير العمل في النظام

### 1. تسجيل المؤجر
- إنشاء حساب وتقديم بياناته الشخصية
- إثبات هويته
- مراجعة البيانات والتحقق منها قبل تفعيل الحساب

### 2. إضافة الأصول
- الدخول إلى لوحة التحكم
- إضافة الأصول (شقة، سيارة، وغيرها)
- تحديد التفاصيل (السعر، الوصف، الصور)
- مراجعة المنصة وقبول أو رفض الأصل قبل عرضه

### 3. تسجيل المستأجر
- إنشاء حساب وتقديم البيانات
- مراجعة وتوثيق البيانات من قبل المنصة
- تصفح الأصول المتاحة بعد تفعيل الحساب

### 4. طلب الاستئجار
- اختيار الأصل المناسب
- إرسال طلب استئجار
- إنشاء طلب داخل النظام وتوجيهه إلى المؤجر

### 5. قبول أو رفض الطلب
- مراجعة المؤجر لبيانات المستأجر
- قبول الطلب أو رفضه
- في حال الرفض: تنتهي العملية
- في حال القبول: الانتقال إلى مرحلة إنشاء العقد

### 6. إنشاء العقد
- إنشاء عقد يحتوي على:
  - بيانات المؤجر والمستأجر
  - تفاصيل الأصل
  - قيمة الإيجار والمدة الزمنية
  - الشروط والأحكام
- عرض العقد على الطرفين
- موافقة الطرفين والتوقيع

### 7. إدارة الدفع
- إنشاء جدول للدفعات (مثل دفعات شهرية)
- قيام المستأجر بالدفع من خلال المنصة
- خصم عمولة المنصة
- تحويل المبلغ المتبقي إلى المؤجر

### 8. متابعة العقد
- متابعة عمليات الدفع
- إرسال تنبيهات في حال التأخير
- تحديث حالة العقد بشكل مستمر
- إنهاء العقد أو تجديده عند انتهاء المدة

---

## النمط المتكرر: عملية القبول والرفض

عند النظر بعمق في سلوك النظام، نلاحظ وجود **نمط متكرر** يتمثل في عملية القبول والرفض، حيث يظهر هذا النمط في عدة مراحل:

| المرحلة | القرار |
|---------|--------|
| قبول حساب المؤجر | مدير النظام يوافق أو يرفض |
| قبول الأصول المضافة | المنصة تقبل أو ترفض |
| قبول طلبات الإيجار | المؤجر يقبل أو يرفض |
| قبول حساب المستأجر | المنصة تقبل أو ترفض |
| الموافقة على العقد | الطرفان يوافقان |

### الدلالة البرمجية

هذا التكرار يشير إلى وجود **مفهوم أساسي داخل النظام** يمكن تجريده كنمط عام يمثل:
- عملية اتخاذ قرار مبني على حالة معينة
- يمكن استثماره في التصميم البرمجي لاحقًا
- توحيد هذه العمليات ضمن سلوك موحد
- تجنب تكرار المنطق بشكل منفصل في كل جزء من النظام

---

## خلاصة

النظام لا يقتصر على عرض الأصول فقط، بل يدير **دورة حياة كاملة** لعملية التأجير من البداية إلى النهاية، مع وجود أنماط متكررة يمكن توحيدها في التصميم البرمجي لتحسين جودة النظام وقابلية صيانته.