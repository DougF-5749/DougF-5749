# 👋 Hello, I'm Doug 👋

I'm a former teacher and education leader with a passion for STEM and a proven ability to communicate complex ideas effectively. After years of honing my skills in logical problem-solving, project management, and collaborative teamwork, I transitioned into the world of **full-stack development**. With a strong foundation in **agile practices** and **user-focused design**, I am now leveraging my experience and technical expertise to build impactful, scalable software solutions.

## 🛠️ Technical SKills 🛠️ 

### Front-End Development

- React.js
- HTML
- CSS

### Back-End Development

- JavaScript
- Node.js
- Express.js
- Python
- SQL (PostgreSQL MySQL)
- NoSQL (MongoDB)
- FastAPI
- Flask

### Data and Analytics

 - Jupyter Notebook
 - pandas
 - NumPy
 <!-- - seaborn
 - matplotlib
 --->

### Testing and QA Tools

- Pytest
- Jest
- Vitest

### Tools and Practices

- Git
- GitHub
- Command Line
- VS Code
- Agile
- Test-Driven Development (TDD)
- Pair Programming

## 🚀 Projects 🚀

### [Rugby Union Internationals: Data Analysis:](https://github.com/DougF-5749/rugby_union_internationals) _(Solo Project - **ongoing**)_

**Tech Stack:** Python, Jupyter Notebook, pandas, NumPy, Matlpotlib, seaborn

 - Conducting data analysis on international rugby matches using Python and pandas.
 - Designing interactive Jupyter Notebooks for exploratory data analysis.
 - Cleaning, transforming, and visualising match statistics using Seaborn and Matplotlib (ongoing)

### [Plucker:](https://github.com/DougF-5749/Plucker/tree/main) _(Group Project - Makers Academy Bootcamp)_

**Tech Stack:** Python, Flask, React, PostgreSQL

- Created a bird identification app with Flask (asynchronous capabilities using Hypercorn and asyncio).
- Integrated humorous functionality by generating random recipes for newly logged bird sightings.

**Impactful Commits:**

**1️⃣ [database design and seed data](https://github.com/DougF-5749/Plucker/commit/2fb293dec3cbeedf5518b76e56b5dcbec596a0e0)**

- This schema is designed for an application where users track bird sightings, and each sighting generates one recipe. Those recipes, in turn, are broken down into ingredients, steps, and ratings.

- To facilitate quick testing, several rows are inserted into each table. This seeded data ensures that we can immediately run queries and evaluate the schema’s functionality without having to create everything manually.

**2️⃣ [db_connection setup](https://github.com/DougF-5749/Plucker/commit/ba244e6308ea69737601f7cc94fb744fffc8fb51)**
- I removed psycopg2 from the requirements and replaced it with asyncpg, allowing the project to use an asynchronous database connection to manage interactions with the database.

- Instead of synchronously opening and closing connections for every request, we benefit from better performance and scalability when handling multiple concurrent requests.

**3️⃣ [Recipe Template and Service Layer](https://github.com/DougF-5749/Plucker/commit/e2417a836594ba6bf32da5ef5ac8156d9ce8aa4d)**

 **Recipe Templates:**
- Early on, the project needed a quick way to generate recipes before we could integrate with an AI API for dynamic recipe generation. As an MVP solution, we decided to **hardcode recipe templates** (eventually 11). One of the first examples was **HERB_GLAZED_RECIPE**
 
- A standardised template ensures every recipe has a clear format (title, cooking time, ingredients, steps) that **aligned with the database design**.

- The **placeholder {BIRD}** lets us easily adapt this base template for any bird name

- While the final goal was to generate recipes on-the-fly via an AI API (with a carefully crafted prompt), **time constraints** led us to maintain a random selection of hardcoded recipes.

 **Service Layer:**
- I learned that basic CRUD operations should live in repository files, while higher-level application logic belongs in a **service layer**. This ensures each layer has a clear responsibility.
  
- I created a **RecipeService class** to handle higher-level functionality like creating a recipe based on a bird sighting.
  - This service depends on repositories for data operations (e.g., saving sightings, recipes, ingredients, steps).
  - It abstracts the flow of creating a recipe (which span multiple tables) into a single method (**_create_recipe_from_bird_name_**).
 
- A **helper function** (**_populate_bird_template_**) inserts the bird name into a predefined recipe template (e.g HERB_GLAZED_RECIPE).

**4️⃣ [Blue print for route abstraction](https://github.com/DougF-5749/Plucker/commit/01f3e58aa1d2568e7104e99b4ab291d75a42058c)**
- This commit is an exmplae of how I abstracted routes into their own routes directory instead of defining routes directly in app.py.

- Each set of related endpoints is organised within a Flask Blueprint. The main app.py file then calls app.register_blueprint() to link these routes together. This avoids clutter in app.py, making it easier to maintain and locate specific endpoints.

- As the project grows, new features (e.g. authentication, recipe endpoints, etc.) can each have their own Blueprint. This pattern reduces merge conflicts and promotes modular development.

### [ThySpace:](https://github.com/DougF-5749/ThySpace) _(Group Project - Makers Academy Bootcamp)_

**Tech Stack:** MongoDB, Express.js, React, Node.js

- Built a medieval-themed social platform replicating Facebook with features like alliances, posts, comments, and likes.

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
