# Juice Shop: Deprecated Interface  

## Challenge Overview  
- **Title:** Deprecated Interface  
- **Difficulty:** 2/6  
- **Description:** Use a deprecated B2B interface that was not properly shut down.  

---

## Tools Used  
- **Browser**  

---

## Methodology and Solution  

The challenge description hinted at a **deprecated interface** still being active in the application.  
This suggested that some **old or unused functionality** might still be accessible.  

---

### 1. Exploring the Application  
- I manually browsed through different sections of the Juice Shop.  
- The **Complaint section** allowed users to upload files.  

---

### 2. Uploading a Suspicious File  
- Normally, the complaint form accepts text/image uploads.  
- I tried uploading a file with an **`.xml` extension**.  
- Surprisingly, the application accepted it without restriction.  

---

### 3. Triggering the Deprecated Interface  
- The system processed the `.xml` file upload, which indicated that a **legacy XML-based B2B interface** was still running in the background.  
- This confirmed the vulnerability.  

---

### 4. Result  
-  Challenge solved – by uploading an XML file, I successfully interacted with the **deprecated interface** that should have been disabled.  

---
