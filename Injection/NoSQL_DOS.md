# Juice Shop: NoSQL DoS  

## Challenge Overview  
- **Title:** NoSQL DoS  
- **Difficulty:** 4/6  
- **Description:** Let the server sleep for some time. (It has done more than enough hard work for you)  

---

## Tools Used  
- **Browser** – To trigger search/review queries.  

---

## Methodology and Solution  

This challenge was a bit tricky at first because I didn’t have much prior experience with **NoSQL injection**. After researching online and experimenting, I realized the goal was to **force the server into sleeping** by injecting a special query.  

---

### 1. Understanding the Vulnerability  
In **NoSQL databases** like MongoDB, user input is often directly embedded in query objects. If not sanitized, it’s possible to inject JavaScript expressions. Some functions, such as `sleep()`, can cause intentional **delays**, simulating a DoS (Denial of Service).  

---

### 2. Crafting the Payload  
In the **product review query**, I injected the following payload directly in url bar:  

```json
{
  http://localhost:3000/rest/products/sleep(1000)/reviews
}
