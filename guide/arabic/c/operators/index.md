---
title: Operators
localeTitle: العاملين
---
# المشغلون في C

## 1\. المشغلين الحساب

*   `+` إضافة إلى المعاملات (القيم) `C int a = 6; int c = a + 1; // c = 7`
*   `-` يطرح المعامل الثاني من الأول `C int a = 8; int b = 9; int c = a - b; // c = -1`
*   `*` ضرب اثنين من المعاملات `C int a = 8; int b = 9; int c = a * b; // c = 72`
*   `/` يقسم المعامل الأول من الثاني `C int a = 8; int b = 4; int c = a / b; // c = 2`
*   `%` يعطي الباقي بعد قسمة عدد صحيح `C int a = 8; int b = 9; int c = b % a; // c = 1 because b = 1*a + 1 = 8 + 1`
*   `++` يزيد قيمة int من قبل واحد `C int a = 8; a++; // a = 9 int b = a++; // postfix operator; a = 10, b = 9 int c = ++a; // prefix operator; a = 11, c = 11`
*   `--` يقلل قيمة int من قبل واحد `C int a = 8; a--; // a = 7 int b = a--; // postfix operator; a = 6, b = 7 int c = --a; // prefix operator; a = 5, c = 5` // C برنامج لإثبات عمل المشغلين الحساب

# تتضمن

انت مين() { int a = 9، b = 4، c؛

 `c = a+b; 
 printf("a+b = %d \n",c); 
 
 c = ab; 
 printf("ab = %d \n",c); 
 
 c = a*b; 
 printf("a*b = %d \n",c); 
 
 c=a/b; 
 printf("a/b = %d \n",c); 
 
 c=a%b; 
 printf("Remainder when a divided by b = %d \n",c); 
 
 return 0; 
` 

}

## 2\. العلاقات العلائقية

*   `==` يساوي - صحيح عندما يساوي المعادلان `C int a = 5, b = 5; bool c = (a == b); // c = true`
*   `!=` لا يساوي - صحيح عندما لا يتساوى المعاملان `C int a = 5, b = 6; bool c = (a != b); // c = true`
*   `>` أكبر من - True عندما يكون المعامل الأول أكبر من الثاني. `C int a = 8, b = 5; bool c = (a > b); // c = true`
*   `<` أقل من - صحيح عندما المعامل الأول هو أصغر ثم الثانية. `C int a = 5, b = 8; bool c = (a < b); // c = true`
*   `>=` أكبر من أو يساوي - True عندما يكون المعامل الأول أكبر أو يساوي الثاني. `C int a = 8, b = 5; bool c = (a >= b); // c = true bool d = (a >= 8); // d = true`
*   `<=` أقل من أو يساوي - صواب عندما يكون المعامل الأول أصغر أو يساوي الثاني. `C int a = 5, b = 8; bool c = (a <= b); // c = true`

## 3\. المنطقية المشغلين

*   `&&` AND operator - عندما يكون **كلا** المعاملين صحيحين. `C bool c = (5 < 6) && (8!=7); // both operands true, therefore c = true`
*   `||` OR operator - True عندما يكون المعامل الأول أو الثاني صحيحًا (أو كليهما) `C bool c = (5 < 6) || (8 == 7) // first operand is true, therefore c = true`
*   `!` NOT operator - True عندما يكون المعامل غير صحيح. `C bool c = !(8 == 7) // translate: NOT (false), therefore c = true`

## 4\. المشغلات bitwise

*   عامل التشغيل `&` AND - إذا كان هناك في مكان ما قليلاً في كلا المعاملات ، فإنه يتم نسخه إلى النتيجة `C A = 11001 B = 01000 RESULT = 01000`
*   `|` عامل التشغيل OR - إذا كان يوجد في مكان ما في أي من المعاملات ، فإنه يتم نسخه إلى النتيجة `C A = 11001 B = 01000 RESULT = 11001`
*   `^` XOR (OR OR) المشغل - إذا كان يوجد في مكان ما في أحد المعاملات (وليس كلاهما) ، فإنه يتم نسخها إلى النتيجة `C A = 11001 B = 01000 RESULT = 10001`
*   `~` عامل النفي - عكس البتات. 1 -> 0 ، 0 -> 1 `C C = 01000 RESULT = 10111`
*   `<<` مشغل Left shift - يتم تحريك المعامل الأيسر يسارًا بواسطة عدد كبير من البتات ، مثل المعامل الصحيح `C A = 11001 A << 2 RESULT = 00100`
*   `>>` مشغّل shift الأيمن - يتم تحريك المعامل الأيسر مباشرة بعدد البتّ ، مثل المعامل الصحيح `C A = 11001 A >> 2 RESULT = 00110`

## 5\. مشغلي التكليف

*   `=` `C int a = 7; // 'a' is going to be equal to 7`
*   `+=` `C int a = 7; a += 5; // equivalent to a = a + 5 = 7 + 5 = 12`
*   `-=` `C int a = 7; a -= 2; // equivalent to a = a - 2 = 7 - 2 = 5`
*   `*=` `C int a = 7; a *= 3; // equivalent to a = a * 3 = 7 * 3 = 21`
*   `/=` `C int a = 21; a /= 3; // equivalent to a = a / 3 = 21 / 3 = 7`
*   `%=`  
    `C int a = 21; a %= 5; // equivalent to a = a % 5 = 21 % 5 = 1`

متفرقات المشغلين ↦ sizeof و ternary إلى جانب المشغلين التي نوقشت أعلاه ، هناك عدد قليل من المشغلين المهمين الآخرين بما في ذلك sizeof و؟ : بدعم من C لغة.

وصف المشغل مثال sizeof () يرجع حجم متغير. sizeof (a) ، حيث a عدد صحيح ، سيعود 4. ويعيد عنوان المتغير. &ا؛ إرجاع العنوان الفعلي للمتغير.

*   مؤشر للمتغير. \*ا؛ ؟ : التعبير الشرطي. إذا كان الشرط صحيح؟ ثم قيمة X: وإلا قيمة Y

## 6\. الأسبقية المشغل في C

يظهر المشغلون ذوو الأسبقية الأعلى في أعلى القائمة. ضمن التعبير ، المشغلين مع الأسبقية العالية سيتم تقييمها أولا.

*   Postfix `() [] -> . ++ --`
*   Unary `+ - ! ~ ++ -- (type)* & sizeof`
*   مضاعف `* / %`
*   مضاف `+ -`
*   التحول `<< >>`
*   العلائقي `< <= > >=`
*   المساواة `== !=`
*   Bitwise AND `&`
*   Bitwise XOR `^`
*   Bitwise OR `|`
*   منطقي و `&&`
*   منطقية أو `||`
*   الشرطي `?:`
*   Assignment `= += -= *= /= %= >>= <<= &= ^= |=`
*   فاصلة `,`