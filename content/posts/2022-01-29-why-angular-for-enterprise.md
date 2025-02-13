---
title: 'لماذا إطار العمل Angular مناسب للمشاريع الكبيرة ؟'
date: 2022-01-29
slug: 'why-angular-for-enterprise'
template: 'post'
categories:
  - javascript
tags:
  - javaScript
  - angular
  - react
  - Vuejs
thumbnail: '../thumbnails/angular.png'
---

من المعروف على **إطار العمل Angular** أنه يستخدم على نطاق واسع من طرف الشركات والمنظمات الإقتصادية الكبيرة لبناء واجهاتها الرسومية. ولعل اقترانه الدائم بلغة Java وبيئة .NET يفسر هذه الحقيقة، حيث أنهما ــ جافا ودوت نت ــ يستخدمان بقوة من طرف تلك الكيانات الكبيرة ونادرا ما تجد لهما وجودا في سوق العمل الحر بالمقارنة مع لغات مثل PHP على سبيل الذكر لا الحصر.

**فما هي إذن الأسباب التي تجعل تلك الشركات تفضل أنجولار** على حساب المنافسين القويين [React](/web-development/javascript/react-javascript-library/) و [Vue](/vuejs-framework/) ؟

> حينما نقول بأن أنجولار معروف ومطلوب للغاية في نطاق ال Enterprise فهذا لا يعني البتة بأن React أو Vue غير مطلوبان في ذلك المجال، بل على العكس هناك وجود لهما في ذلك المجال ولكن من واقع خبرتي وتجربتي وجود Angular يطغى عليهما.

## السبب الأول: أنجولار إطار عمل

السبب الأول هو كون [Angular](/web-development/javascript/components-angular-framework/) إطار عمل بالمعنى الحرفي في حين أن React و Vue لوحدهما تعتبران مجرد مكتبات لبناء ال UI.
إطار العمل يعني أنه يوفر كل ما تحتاجه في المشروع:

- Router
- Structure (Modules, DI, RxJS ...)
- Http client - في أنجولار لن تحتاج للتفكير على ستسخدم `axios` أم حل آخر للقيام ب Http Request.
- Automated Testing
- ...

هذا يعني أنه عندما يتم توظيف شخص فالمفترض أنه على علم وخبرة بكل هذه الأمور والأدوات. على عكس React مثلا، قد يعتمد المشروع في State Management على Redux بينما الشخص الجديد لديه خبرة في MobX أو Recoil. يعني ذلك أنه سيحتاج لبعض الوقت للإندماج في الفريق وتعلم تلك التقنيات الجديدة، والوقت عند تلك الشركات يساوي المال 💵

## السبب الثاني: TypeScript

يعتمد Angular بشكل أساسي على لغة البرمجة TypeScript وميزتها الأساسية المتمثلة في Type Checking. فالمعلوم أن كل المشاريع الكبرى والتي تطور باستمرار تفضل الإستعانة بلغات مثل Java أو C# تدعم Type Checking لسهولة قراءة الكود وتقليص فرص ظهور الأخطاء في Runtime، وهو ما يوفره TypeScript.

## السبب الثالث: Automated testing

منذ اليوم الأول جعل Angular [الإختبارات البرمجية](/web-development/ما-هي-الإختبارات-البرمجية/) من أولوياته، وبالتالي فهو مُعَدٌّ خصيصا من أجلها ويوفر أوامر سطرية جاهزة لتوليدها وتنفيذها. كما أنه يسهل بشكل كبير إدخالها في عمليات CI/CD.

## السبب الرابع: الدعم طويل الأمد (Long Term Support)

كل شركة تبدأ في مشروع يكلفها ميزانيات كبيرة تريد أن تطمئن على مستقبل ذلك المشروع، وإطار عمل مثل أنجولار يوفر هذه الضمانات كونه يشرف على دعم وتطوير كل الأدوات المنضوية تحت لواء أنجولار.

على عكس React مثلا، فقد يكون دعم المكتبة نفسها جيدا وطويل الأمد ولكن ليس هناك ضمانات على أن دعم Redux مثلا سيستمر وقتا طويلا.

## السبب الخامس: الرخصة

هذا من الأسباب المهمة كذلك، حيث أن أنجولار كان منذ ميلاده تحت رخصة MIT التي لا تشترط على المستهلكين أية أمور من شأنها أن تسبب لهم القلق.

بينما مكتبة React كانت إلى وقت قريب تعتمد رخصة BSD + Patent التي سببت لها الكثير من المشاكل مع مستخدمين كبار لعل أهمهم منصة إدارة المحتوى ووردبريس التي [صرح المسؤولون عنها أنهم غير مرتاحون مع تلك الرخصة](https://ma.tt/2017/09/on-react-and-wordpress/) حينما كانوا قيد دراسة استخدام React في مشروع Gutenberg. بعدها، وفي سبتمبر من عام 2017، أذعن المشرفون على React لتلك الضغوطات وأعلنوا تخليهم عن BSD + Patent لصالح MIT.

<Author slug="aissa" />
