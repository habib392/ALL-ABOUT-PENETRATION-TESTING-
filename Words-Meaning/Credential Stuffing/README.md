## Credential Stuffing hota kya hai?

Yeh ek dangerous technique hai jahan attacker:
Puri ek bari list (dictionary) use karta hai jo username aur password pairs ka hoti hai.
Yeh pairs real logon ke hotay hain jo pehle kisi website se hack ho chuke hote hain (data breach mein leak hua data).
Log aksar ek hi password har website pe reuse karte hain, isliye attacker sochta hai:
"Shaayad yeh same password is nayi website pe bhi kaam kar jaye."

**🧪 Kaise kaam karta hai?**
Hacker har username:password pair sirf aik baar try karta hai.
To account locking system activate hi nahi hota, kyunke woh sirf multiple failed attempts par trigger hota hai.
Lekin agar kisi bhi pair ka combination match kar gaya — to attacker uska account le jaata hai.

**😨 Yeh attack khatarnaak kyun hai?**
Automated tools se yeh sab kuch fast ho jaata hai.
Sirf ek run mein 100s ya 1000s of accounts hack ho sakte hain.
Aur victim ko pata bhi nahi chalta kyunke har username bas aik baar test hua hota hai.

Asan alfaz main Pitchfork attack same credential stuffing ki tarah hi hai

## Example:
Agar tumhare paas ye values hain:

Usernames: admin, 21322, rock, dave

Passwords: khan, sadwq, jack, hary

To Pitchfork attack inko line-by-line match karega:

Attempt No.	Username	Password
- (1)	admin	khan
- (2)  21322	sadwq
- (3)	rock	jack
- (4)	dave	hary
