---
title: "התקנת סביבת עבודה"
date: 2021-03-14T19:42:02Z
tags:
- go
- מדריכים
categories: []
authors:
- avi 
---

להתקנה בווינודס אפשר לחפש את ההוראות התקנה [כאן](https://golang.org/doc/install)
בלינוקס הכי פשוט להשתמש בסקריפט הבא
```
wget -q -O - https://raw.githubusercontent.com/canha/golang-tools-install-script/master/goinstall.sh | bash

```
ולפעול לפי ההוראות.  
אפשר לבדוק האם זה הותקן בהצלחה עם
```
go version
```
הסקריפט הנ"ל מתקין את GO  
ויוצר את התיקייה GO   
(ששם נבנה את כל האפליקציות שלנו) בתיקיית המשתמש.

תחת התיקייה GO יש 3 תיקיות:  
src - התיקייה בו אתם תשמרו את כל הקוד שלכם.  
pkg - התיקייה מתחתיה נמצאים קבצים מקומפלים וכן החבילות הרלוונטיות למערכת הפעלה שלכם (GO מתקפל בקלות לכל מערכות ההפעלה בלי צורך בשינוי בקוד, אבל כיוון שיש API אחר לכל מערכת הפעלה צריך את החבילות האלו, אבל לא נראה לי שיש למשתמש הפשוט משהו לשנות שם) אם מישהו יכול להסביר יותר מה קורה בתיקיה הזאת נשמח לשמוע .  
bin - התיקייה אליה נשלחים הקבצים המקופלים (אפליקציה אותה ניתן להריץ בפועל).   

נ.ב. למי שרוצה לשחק קצת עם הקוד בלי להתקין אפשר להתנסות [כאן](https://goplay.x1unix.com/)
