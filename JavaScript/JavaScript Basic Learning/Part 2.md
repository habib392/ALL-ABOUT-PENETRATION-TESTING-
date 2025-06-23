

1. ✅ prompt("Enter your age")
Sahi kaha — yeh user ko ek pop-up box dikhata hai browser mein jahan user apni age likhta hai.
Example: 19, 16, etc.


2. ❌ console.log() website par output nahi dikhata
🔁 Correction:
console.log("User entered age:", age) ka output developer tools ke "Console" tab mein aata hai, na ke user ko dikhai deta hai.
Yeh penetration testers aur developers background mein debugging ke liye use karte hain.


3. ✅ if (age >= 18)
Sahi — agar user ne 18 ya 19 ya zyada age daali, to alert("You are an adult!") chalta hai.
Yeh website pe pop-up hota hai — user ko dikhai deta hai.


4. ✅ else condition
Agar age 18 se kam hai, to alert("You are underage!") chalta hai.
Yeh bhi pop-up hai user ke liye.




---

📌 Final Flow in Your Zuban:

Page pe button hai → "Check Your Age"

Jab banda click karega:

Usko ek box milega → "Enter your age"

User likhega: 19

Console mein developer ko dikhai dega: "User entered age: 19"

Agar age 18 ya zyada hai → user ko alert: "You are an adult"

Agar age 18 se kam hai → user ko alert: "You are underage"




---

💻 Hacker ya XSS ky angle se?

Hacker agar XSS payload daalta hai jo prompt() ya alert() chalaye, to wo check karta hai:

Page pe script execute ho rahi hai ya nahi?

Agar haan → vulnerability confirmed
