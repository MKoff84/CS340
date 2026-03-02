CS 340 – Client/Server Development
Module Eight Reflection
Writing Maintainable, Readable, and Adaptable Programs

Writing maintainable, readable, and adaptable programs begins with clear structure and separation of concerns. In Project One, I developed a dedicated CRUD Python module responsible solely for handling database operations. This module isolated database connection logic and query methods from the dashboard interface built in Project Two.

By separating the data access layer from the presentation layer:

--The dashboard code remained clean and focused only on user interaction.

--Database logic could be modified without affecting the user interface.

--Debugging became easier because responsibilities were clearly divided.

This modular design made Project Two significantly more efficient to implement. Instead of embedding database queries directly into dashboard callbacks, the application simply called methods from the CRUD module.

Advantages of This Approach

--Improved readability – Each file has a single responsibility.

--Better maintainability – Changes to the database logic require edits in only one location.

--Reusability – The CRUD module can be reused across multiple projects.

Future Use of the CRUD Module

This CRUD module could be reused in:

--A web-based administrative portal

--A REST API backend service

--A mobile application backend

--A data analytics or reporting system

Because the module abstracts MongoDB interactions, it serves as a reusable data access layer for future systems.

Approaching Problems as a Computer Scientist

--As a computer scientist, I approach problems by:

--Analyzing requirements carefully.

--Breaking the system into logical components.

--Designing data structures to support expected operations.

Testing incrementally and refining based on results.

For this project, I first studied the database structure and identified how specific fields (breed, age, rescue type, location) could support Grazioso Salvare’s operational needs. I then designed MongoDB queries to filter animals appropriately before integrating those queries into dashboard callbacks.

How This Differed From Previous Assignments

Unlike many prior assignments that focused on isolated algorithms or theoretical exercises, this project required full-system thinking:

--Database design

--Backend logic implementation

--Frontend dashboard integration

--Real-time data interaction

This experience emphasized architectural planning rather than single-function problem solving.

Strategies for Future Database Design

In future projects involving client requirements, I would:

--Begin with structured requirement analysis.

--Design schemas around anticipated query patterns.

--Use embedded documents intentionally where beneficial.

--Prototype aggregation pipelines early.

--Maintain strict separation between data access and UI logic.

This systems-oriented approach improves scalability, performance, and long-term adaptability.

What Computer Scientists Do and Why It Matters

Computer scientists design systems that convert raw data into meaningful, actionable information.

In this project, the database contained thousands of animal records. Without structured queries, filtering, and visualization tools, that data would remain underutilized. By building a CRUD module and interactive dashboard, I created a system that enables Grazioso Salvare to:

--Filter animals by rescue category

--Analyze breed distribution trends

--Visualize geographic data

--Make informed operational decisions

This work matters because organizations increasingly rely on data-driven decision-making. Efficient systems reduce manual processes, increase clarity, and support strategic planning.

Through projects like this, computer scientists provide the technical infrastructure that allows companies to operate more intelligently, efficiently, and effectively.candidates and understand patterns within their data.

Ultimately, computer scientists build the infrastructure that allows organizations to operate smarter, faster, and more strategically.
