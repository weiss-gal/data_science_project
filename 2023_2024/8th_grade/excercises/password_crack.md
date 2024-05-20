# משימת פיצוח הסיסמא

המשימה שלכם, אם תבחרו לקבל אותה, היא לפצח את הסיסמא בתכנה הבאה:

https://github.com/weiss-gal/data_science_project/blob/main/2023_2024/10th_grade/excercises/password_crack.py

כדי להתחיל, הורידו את התכנה ונסו להריץ אותה פעם או פעמיים.

הערה - יכול להיות שכדי להריץ אותה תזדקקו להתקין ספריות מסויימות, אם תתקלו בשגיאה מסוג זה תצטרכו להתקין את הספרייה cryptography, כדי לעשות זאת עליכם לפתוח את שורת הפקודה של windows (לחצו על מקש מיקרוסופט פעם אחת, הקלידו את המילה `cmd` ואז enter) ולהפעיל את הפקודה הבאה:

`python -m pip install cryptography`

דבר ראשון - אל תבהלו מגודל הקוד, רובו לא באמת מעניין אתכם.
אחרי שתריצו את התכנה פעם או פעמיים תראו שאי אפשר באמת להתקדם בלי הסיסמה. הייתי שמח לעזור לכם אבל לצערי שכחתי את הסיסמה. 

## אז מה עושים
בתור הקוד יש מחרוזת ארוכה שנראת כמו ערימת קללות בסנסקריט, זה לא ערימת קללות, זהו מסר מוצפן. כדי לפענח (decrypt) את המסר נדרשת סיסמא, את הסיסמא הופכים למפתח באמצעות הפונקציה `derive_key` ואז אפשר לקרוא לפונקציה `decrypt_text` עם המסר המוצפן והמפתח. 
אתם יכולים לשנות את התכנה ככה שהיא תנסה מספר סיסמאות ככל שתרצו (זכרו מה למדנו על brute force) עד שתמצאו את הסיסמה הנכונה. רק זכרו שכל ניסוי לפתוח את המסר באמצעות מפתח כלשהו לוקח זמן (קצר מאוד, אבל עדיין לוקח). זאת אומרת שלנסות סיסמא אחת או שתיים יקח אפס זמן, אבל אם תנסו מליון סיסמאות שונות ... זה כבר יכול לקחת שעות. אז כדאי לחשוב טוב איזה סיסמאות אתם רוצים לנסות. מנסיוני - אם תכתבו נכון את הbrute-force שלכם, התכנה תפצח את הסיסמא הנכונה בתוך דקה שתיים.

## עוד שנייה, נזכרתי במשהו

- הסיסמה היא מחרוזת שמייצגת תאריך במבנה הבא DDMMYYYY . זאת אומרת שתי ספרות ליום, שתי ספרות לחודש וארבע ספרות לשנה, למשל ה27 לינואר 2024 הוא 27012024
- הסיסמה היא התאריך לידה של הכלבה שלי, תהא מנוחתה עדן, שנפטרה לפני כמה חודשים.

עכשיו באמת אתם יודעים כל מה שצריך, בהצלחה 

_ההודעה הזו לא תשמיד את עצמה בעוד שלושים שניות, זה היה יכול להיות מגניב אבל הביטוח של בית הספר מתנגד לכך_