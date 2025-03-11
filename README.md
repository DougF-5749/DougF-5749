# 👋 Hello, I'm Doug 👋

I'm a former teacher and education leader with a passion for STEM and a proven ability to communicate complex ideas effectively. After years of honing my skills in logical problem-solving, project management, and collaborative teamwork, I transitioned into the world of **software development**. With a strong foundation in **agile practices** and **user-focused design**, I am now leveraging my experience and technical expertise to build impactful, scalable software solutions.

## Project Contents
1. [Ongoing Projects](#ongoing-projects)
2. [Completed Projects](#completed-projects)

## 🛠️ Technical Skills and Tools 🛠️ 

### Front-End Development
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### Back-End Development
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)

### Data and Analytics
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

### Testing and QA Tools
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)

### Tools and Practices
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Command Line](https://img.shields.io/badge/CLI-4A90E2?style=for-the-badge&logo=windows-terminal&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Agile](https://img.shields.io/badge/Agile-29ABE2?style=for-the-badge&logo=agile&logoColor=white)
![TDD](https://img.shields.io/badge/Test--Driven_Development-FF7139?style=for-the-badge&logo=testing-library&logoColor=white)
![Pair Programming](https://img.shields.io/badge/Pair_Programming-FFD700?style=for-the-badge&logo=teams&logoColor=black)

## Ongoing Projects

### [Solar System Travel - SQL Project](https://github.com/DougF-5749/space_travel) _(Solo Project)_

**Tech Stack:** Python, PostgreSQL, Astropy

- Designing an SQL database to manage space travel routes and spacecraft data.
- Implementing travel time calculations based on spacecraft speeds and changing planetary positions.
- Using Astropy to compute real-time interplanetary distances and adjust route feasibility.

### [Rugby Union Internationals: Data Analysis:](https://github.com/DougF-5749/rugby_union_internationals) _(Solo Project)_

**Tech Stack:** Python, Jupyter Notebook, pandas, NumPy, Matlpotlib, seaborn

 - Conducting data analysis on international rugby matches using Python and pandas.
 - Designing interactive Jupyter Notebooks for exploratory data analysis.
 - Cleaning, transforming, and visualising match statistics using Seaborn and Matplotlib (ongoing)

## Completed Projects

### [Plucker:](https://github.com/DougF-5749/Plucker/tree/main) _(Group Project - Makers Academy Bootcamp)_

**Tech Stack:** Python, Flask, React, PostgreSQL

**Overview:** 
- Created a **bird identification** app with Flask (asynchronous capabilities using Hypercorn and asyncio).
- Integrated culinary functionality by **generating random recipes** for newly logged bird sightings.

**Impactful Commits:**

**1️⃣ [Database Design and Seed Data](https://github.com/DougF-5749/Plucker/commit/2fb293dec3cbeedf5518b76e56b5dcbec596a0e0)**

- This schema is designed for an application where users track bird sightings, and each sighting generates one recipe. Those recipes, in turn, are broken down into ingredients, steps, and ratings.

- To facilitate quick testing, several rows are inserted into each table. This seeded data ensures that we can immediately run queries and evaluate the schema’s functionality without having to create everything manually.

**2️⃣ [Recipe Template and Service Layer](https://github.com/DougF-5749/Plucker/commit/e2417a836594ba6bf32da5ef5ac8156d9ce8aa4d)**

- **Recipe Templates:**
  - Early on, the project needed a quick way to generate recipes before we could integrate with an AI API for dynamic recipe generation. As an MVP solution, we decided to **hardcode recipe templates** (eventually 11). One of the first examples was **HERB_GLAZED_RECIPE**
 
  - A standardised template ensures every recipe has a clear format (title, cooking time, ingredients, steps) that **aligned with the database design** (see next impactful commit).

  - The **placeholder {BIRD}** lets us easily adapt this base template for any bird name

  - While the final goal was to generate recipes on-the-fly via an AI API (with a carefully crafted prompt), **time constraints** led us to maintain a random selection of hardcoded recipes.

- **Service Layer:**
  - I learned that basic CRUD operations should live in repository files, while higher-level application logic belongs in a **service layer**. This ensures each layer has a clear responsibility.
  
  - I created a **RecipeService class** to handle higher-level functionality like creating a recipe based on a bird sighting.
    - This service depends on repositories for data operations (e.g., saving sightings, recipes, ingredients, steps).
    - It abstracts the flow of creating a recipe (which span multiple tables) into a single method (**_create_recipe_from_bird_name_**).
 
  - A **helper function** (**_populate_bird_template_**) inserts the bird name into a predefined recipe template (e.g HERB_GLAZED_RECIPE).

**3️⃣ [db_connection Setup](https://github.com/DougF-5749/Plucker/commit/ba244e6308ea69737601f7cc94fb744fffc8fb51)**
- I removed psycopg2 from the requirements and replaced it with asyncpg, allowing the project to use an asynchronous database connection to manage interactions with the database.

- Instead of synchronously opening and closing connections for every request, we benefit from better performance and scalability when handling multiple concurrent requests.


**4️⃣ [Blueprint for Route Abstraction](https://github.com/DougF-5749/Plucker/commit/01f3e58aa1d2568e7104e99b4ab291d75a42058c)**
- This commit is an exmplae of how I abstracted routes into their own routes directory instead of defining routes directly in app.py.

- Each set of related endpoints is organised within a Flask Blueprint. The main app.py file then calls app.register_blueprint() to link these routes together. This avoids clutter in app.py, making it easier to maintain and locate specific endpoints.

- As the project grows, new features (e.g. authentication, recipe endpoints, etc.) can each have their own Blueprint. This pattern reduces merge conflicts and promotes modular development.

### [ThySpace:](https://github.com/DougF-5749/ThySpace) _(Group Project - Makers Academy Bootcamp)_

**Tech Stack:** MongoDB, Express.js, React, Node.js

**Overview:** Built a medieval-themed social platform replicating Facebook with features like alliances, posts, comments, and likes.

**Impactful Commits:**

**1️⃣ [Password hashing](https://github.com/SholaF1/acebook_project/commit/ff219f7762c096f5c1ad1d49f3fd908cf12ad656)**
- This commit introduces secure password handling for user accounts by adding password hashing using **bcrypt**. A pre-save hook automatically salts and hashes the user’s plaintext password before saving it to the database to ensure plaintext passwords are never stored directly.

- A **.comparePassword() method** is added to the schema, allowing for safe password verification (e.g., during login).

- bcrypt is added to package.json and installed (package-lock.json updates reflect this).

- A .env-driven **salt-rounds configuration** is introduced to control how many times the password is hashed.

- User **model tests are updated** to verify that the password is stored as a hash and can be compared with a known plaintext (e.g., "password").

**2️⃣ [Comment service functions](https://github.com/SholaF1/acebook_project/commit/a4249e5784fca556f48a326c8263b3712069f752)**
- This commit provides a centralised, test-driven approach to **create**, **update**, and **delete** comments from the front end.
  - **createComment** – Sends a **POST request** to create a new comment on a specific post.
  - **deleteComment** – Sends a **DELETE request** to remove a comment from a post.
  - **updateComment** – Sends a **PUT request** to modify an existing comment on a post.
 
- Each function:
  - Retrieves the backend URL from **environment variables** (import.meta.env.VITE_BACKEND_URL).
  - Includes an authorisation header (Bearer token) to ensure only authenticated users can create, delete, or update comments.
  - Checks for the correct HTTP status codes (201 for creation, 202 for update/delete) and **throws an error** if the response code is unexpected.

- Front end tests with Vitest mock the fetch calls to simulate backend responses and verifying that each request is correctly formed.

**3️⃣ [Email validation](https://github.com/SholaF1/acebook_project/commit/096bd7c82a76c2bda207ae5cc8a229e4f7b8f13e)**
- This commit enhances the sign-up flow by adding consistent email validation in both front-end and back-end layers, improving user experience and security for the registration process.

- The **emailValidator.js** file checks that the email fits a Regex before user creation. If it’s invalid, the middleware responds with an error (400 Bad Request), blocking the registration flow on the backend.
  - **router.post("/", emailValidator, UsersController.createUser)** in **users.js** ensures that any POST to /users must pass email validation before creating a user

- The **SignupPage.jsx** file contains a matching regex check (emailRegex) is used to display an error message (emailErrorMessage) directly to the user if the email format is invalid to provide **immediate feedback** to the user instead of waiting for the server response. A corresponding **.error-message style** is added in SignupPage.css to visually highlight any invalid input.

- By validating on both front-end and back-end, the application prevents invalid email submissions early (**improving user experience**) while also **enforcing stricter data integrit**y at the server level. The user sees a helpful error message if the email is invalid, and the request won’t reach the database at all unless it meets the validation criteria.

<!--
### [FitHub:](https://github.com/DougF-5749/exercise_habit_tracker) _(Solo Project - on hold)_

**Tech Stack:** Python, FastAPI, MySQL

- Developing a backend-focused habit tracker with FastAPI and MySQL, allowing users to securely log workouts.
- Features include user authentication and password hashing.
-->

## 📫 Let's connect 📫

**LinkedIn:** [linkedin.com/in/doug-fairfield](linkedin.com/in/doug-fairfield)

**GitHub:** [github.com/DougF-5749](github.com/DougF-5749)

<!--
**DougF-5749/DougF-5749** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
