# WHAT IS GET/ POST
GET aur POST do common HTTP request methods hain jo browser server se baat karne ke liye use karta hai.
GET request URL mein data bhejti hai jabke POST data ko form body mein chhupa kar bhejti hai.

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
Content-Type: application/x-www-form-urlencoded

username=admin&password=123456**

📌 Data body mein hai, URL mein kuch nahi → POST

### ✅ 3. Contact form (Name, Message) – POST

**POST /contact HTTP/1.1
Host: example.com

name=Habib&message=Hello+admin**

📌 Form se bheja gaya data hidden hai → POST

### ✅ 4. Product filter – GET Request

**GET /products?category=shoes&sort=price HTTP/1.1**

📌 Filter options URL mein dikh rahe hain → GET

### ✅ 5. Signup form – POST Request

**POST /register HTTP/1.1

username=habib123&email=habib@gmail.com&password=abc123**

📌 Sensitive data ja raha hai → chhupa hota hai → POST

## Inn examples sy yeh samj aaya 

Agar BurpSuite mein intercept on karke dekha jaye aur URL mein sirf /login ho lekin neeche body mein username=habib&password=123,
toh woh POST hai.

Agar URL hi kuch aisa ho:
/search?query=testing&sort=latest
toh woh GET hai.

Burpsuite sy sub kuch dekh jaata hai

SUB SY ASAN TARIQA SAMAJNY KA YEH HAI 
GET/POST dono ko data submit krny ky liye use kiya jaata hai 
GET main data url main show hoo jata hai ky kya sumbit hoo rha hai lekin POST main show nhi hota