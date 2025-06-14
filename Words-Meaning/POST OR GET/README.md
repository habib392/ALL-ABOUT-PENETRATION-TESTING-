# WHAT IS GET/ POST
GET aur POST do common HTTP request methods hain jo browser server se baat karne ke liye use karta hai.
GET request URL mein data bhejti hai (visible hota hai) jabke POST data ko form body mein chhupa kar bhejti hai (hidden hota hai).
GET faster hoti hai lekin less secure hoti hai, POST secure hoti hai kyunki sensitive data chhup jata hai.

**GET mein data dikhai deta hai, POST mein nahi**

## EXAMPLES

🔟 System-Based GET vs POST Examples (Burp Style)


### ✅ 1. Search bar – GET Request

**GET /search?query=books HTTP/1.1
Host: example.com**

📌 Data (query=books) URL mein dikh raha hai → GET

### ✅ 2. Login form – POST Request

**POST /login HTTP/1.1
Host: example.com
Content-Type: application/x-www-form-urlencoded**

username=admin&password=123456

📌 Data body mein hai, URL mein kuch nahi → POST

### ✅ 3. Contact form (Name, Message) – POST

**POST /contact HTTP/1.1
Host: example.com**

name=Habib&message=Hello+admin

📌 Form se bheja gaya data hidden hai → POST

