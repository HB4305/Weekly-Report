# Weekly Report

## General Information

**Group ID:** 03  
**Project Name:** Yum Recipe  
**Date Range:** 2026-03-01 – 2026-03-07  


## Tasks Completed This Week

### 23127122 - Nguyễn Duy Thịnh
- Initializing Spring Boot server
- Setting up Liquibase database migration
<details>
<summary>Evidence</summary>

![Commit Messages](ref/initSB.png)

</details>

### 23127205 - Lâm Hữu Khánh
- Built the basic authentication skeleton for the Spring Boot server, including the User entity, UserRepository, and AuthRequest DTO.
- Configured Spring Security (disabled CSRF, permitted public endpoints) and added JWT dependencies.
- Created the AuthController with basic RESTful APIs for registration (/api/auth/register) and login (/api/auth/login).
<details>
<summary>Evidence</summary>

![Authentication Skeleton](ref/skeleton.png)
![Register Successfully](ref/registerAPI.png)
![Login Successfully](ref/loginAPI.png)

</details>

### 23127326 - Lê Mai Hoài Bảo
- Check and redesign the Recipe tables in the database to ensure they are correct.
- Insert sample data into the tables related to Recipes to facilitate API development.

<details>
<summary>Evidence</summary>
- Because I was initially tasked with creating the Recipe tables in the database, but the database creator had already created them, I will review and redesign them if I find anything illogical.

![CheckList](ref/checklist.png)

- After checking and redesigning the tables, I will insert sample data into them to support the development of APIs related to Recipes.
![InsertData](ref/insertdata.png)

- Commit messages for the above tasks:
![Commit Messages](ref/redesignDB.png)

</details>

### 23127357 - Lê Anh Duy
- Create Figma design prototype using Stich and ChatGPT.
- Implementing fridge manager group feature (show, create).
- Implementing Gemini API config and normalize the response from it.
- Implementing the suggest strategy (request -> lookup current ingredients in the fridge -> lookup 20 match recipe -> ask Gemini for the best result -> normalize the response -> response the suggestion for user).

<details>
<summary>Evidence</summary>

![Commit Message](refs/d1.png)

![Commit Message](refs/d2.png)

![Commit Message](refs/d3.png)

![Commit Message](refs/d4.png)

</details>

## AI Usage Declaration

## Tasks Planned for Next Week

### 23127122 - Nguyễn Duy Thịnh
- Implement API enndpoints for Following systems.
- Create the Android app's basic UI for following feed.

### 23127205 - Lâm Hữu Khánh
- Finalize security logic on the Server: Write code to generate and validate actual JWT strings instead of simulated data.
- API Integration: Configure the Retrofit library on Android to make authentication API calls to the Spring Boot server and store the JWT token locally.

### 23127326 - Lê Mai Hoài Bảo
- Implement API to search for recipes based on name, ingredients, and difficulty level.
- Implement API to retrieve detailed information about a specific recipe.

### 23127357 - Lê Anh Duy
- Setup Dependencies Injection.
- Implement AI dish suggestion (backend for sure, frontend if have enough time).

## Issues