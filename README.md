[مساعدة محرر UITk

تحتوي هذه الحزمة على عناصر أدوات واجهة المستخدم وأدوات مساعدة لواجهات المحرر المخصصة في Unity.


راجع تثبيت حزمة من عنوان URL الخاص بـ Git لتثبيتها باستخدام مدير الحزم. عنوان URL الخاص بـ Git لهذه الحزمة هو https://meslubi2021.github.io/Assistant-Editor-UITK/.

يمكنك أيضًا تنزيل هذه الحزمة إلى مجلد الأصول الخاص بك.

نبذة مختصرة عن هذه الحزمة

قم بزيارة وثائق واجهة برمجة التطبيقات الخاصة بالحزمة للحصول على مزيد من المعلومات. انقر فوق اسم للانتقال إلى صفحة الوثائق ذات الصلة للحصول على معلومات الاستخدام وبعض أمثلة التعليمات البرمجية:

علامة قابلة للتحرير

علامة تتحول إلى حقل لتحرير نصها. ويمكن تحريرها بنقرة مزدوجة افتراضيًا.

معاينة EditableLabel

عرض علامات التبويب

عنصر من عناصر مجموعة أدوات واجهة المستخدم لتنظيم المحتوى باستخدام علامات التبويب. يتوفر به خيار دعم فتح علامات تبويب متعددة في نفس الوقت من خلال الضغط على shift أو ctrl (أو cmd في نظام التشغيل macOS) أثناء النقر فوق علامة تبويب. كما يدعم تذكر علامات التبويب المفتوحة الأخيرة من خلال تعيين سلسلة فريدة كمفتاح استمرار.

معاينة TabbedView

حقل خصائص المصفوفة

عنصر تحكم UITK لمجموعة أو قائمة متسلسلة. يحتوي على العديد من خيارات التخصيص.

معاينة ArrayPropertyField

قائمة المفتشين

قائمة من الكائنات تشبه قائمة المكونات في مفتش GameObject. يُستخدم هذا العنصر عادةً مع قائمة من الأصول الفرعية.

معاينة ListOfInspectors

حاوية الملكية

عنصر يعرض مؤشرات تجاوز مسبقة الصنع لـ SerializedProperty وقائمة سياق الخاصية. حاليًا، يعرض Unity هذه الأشياء فقط لبعض الحقول المحددة في ظل ظروف محددة. يجعل هذا العنصر هذه الميزات متاحة في كل مكان.

حقل مرجعي مُدار

يدعم SerializeReference قبل 2022.2. يضيف Unity 2022.2 دعمًا للمراجع المُدارة في UITK، ولكن لا يزال هذا العنصر مفيدًا هناك للتغلب على بعض الأخطاء (على سبيل المثال، لا يحب UITK احتواء فئتين على حقول بنفس الاسم ولكن من نوع مختلف).

قائمة مخصصة للمراجع المُدارة

سدادة الربط

عنصر يمنع ربط العناصر التابعة له بعناصر أعلى في التسلسل الهرمي. استخدم هذا العنصر للاحتفاظ بالحقول المرتبطة بعناصر مختلفة عن بقية واجهة المستخدم.

مُعطل

عنصر يقوم بتعطيل محتواه وفقًا لاستدعاء. وهو مشابه لـ DisabledScope في IMGUI .

المساحة الثابتة والمساحة المرنة

عناصر لإضافة مسافة بسرعة على طول اتجاه مرونة العنصر الأصلي. وهي تشبه عنصري Space و FlexibleSpace في IMGUI .

أداة السحب والنقر

معالج يتولى التعامل مع النقرة باعتبارها سحبًا عند سحب الماوس، وكنقرة عند النقر فوق الماوس دون تحريكه. وهو مفيد للأشياء التي يمكن النقر عليها وسحبها، مثل رؤوس المكونات في المفتش.

ملحقات الكائنات المتسلسلة

طرق التمديد لـ SerializedObject مفيدة بشكل خاص عند استخدامها مع UI Toolkit. تحتوي على طريقة IsEditable التي يمكن استخدامها مع عنصر Disabler لتجنب تحرير الكائنات التي لا ينبغي تحريرها

ملحقات مجموعة أدوات واجهة المستخدم

يحتوي على العديد من طرق التمديد لعناصر VisualElements. فهو يحتوي على طرق للتعامل فقط مع العناصر الفرعية المباشرة لعنصر، وبعض الطرق الأخرى لتعيين خصائص نمط متعددة بسرعة في وقت واحد، وطريقة للحصول على SerializedProperty المرتبطة بحقل، من بين أشياء أخرى.

هام: تضمين هذه الحزمة

إذا كنت تنوي تضمين هذه الحزمة داخل حزمة أخرى أو مكون إضافي لـ Asset Store، فيرجى اتباع الخطوات التالية لتجنب الاصطدامات في المشاريع التي تستخدم هذه الحزمة بمفردها.
