# Clean-Architecture

𝗪𝗵𝗮𝘁 𝗶𝘀 𝗖𝗹𝗲𝗮𝗻 𝗔𝗿𝗰𝗵𝗶𝘁𝗲𝗰𝘁𝘂𝗿𝗲?

The Clean Architecture philosophy emphasizes the importance of separating concerns in software design and creating code that is 𝗺𝗼𝗱𝘂𝗹𝗮𝗿, 𝘁𝗲𝘀𝘁𝗮𝗯𝗹𝗲, 𝗮𝗻𝗱 𝗺𝗮𝗶𝗻𝘁𝗮𝗶𝗻𝗮𝗯𝗹𝗲. It is developed by software engineer and consultant Robert C. Martin.
 
At its core, Clean Architecture promotes the idea that software systems should be designed with the primary goal of 𝗯𝗲𝗶𝗻𝗴 𝘂𝗻𝗱𝗲𝗿𝘀𝘁𝗼𝗼𝗱 𝗮𝗻𝗱 𝗺𝗮𝗶𝗻𝘁𝗮𝗶𝗻𝗲𝗱 𝗯𝘆 𝗱𝗲𝘃𝗲𝗹𝗼𝗽𝗲𝗿𝘀 over the long term.

To achieve this goal, Clean Architecture proposes a layered architecture with 𝗰𝗹𝗲𝗮𝗿 𝗯𝗼𝘂𝗻𝗱𝗮𝗿𝗶𝗲𝘀 𝗯𝗲𝘁𝘄𝗲𝗲𝗻 𝗱𝗶𝗳𝗳𝗲𝗿𝗲𝗻𝘁 𝗰𝗼𝗺𝗽𝗼𝗻𝗲𝗻𝘁𝘀 𝗼𝗳 𝘁𝗵𝗲 𝘀𝘆𝘀𝘁𝗲𝗺, so we can achieve independence of frameworks, UI, databases, and delivery mechanisms, as well as the possibility to test in isolation.

The Clean Architecture philosophy defines a 𝘀𝗲𝘁 𝗼𝗳 𝗹𝗮𝘆𝗲𝗿𝘀, starting with the most general and abstract layers and moving toward the most concrete and specific layers. These layers include:

🔹 𝗘𝗻𝘁𝗶𝘁𝗶𝗲𝘀: The fundamental objects in the system, which represent the core business logic and data. They encapsulate the most general and high-level rules.

🔹 𝗨𝘀𝗲 𝗰𝗮𝘀𝗲𝘀: The high-level interactions between the system and its users or other external systems, containing application-specific business rules. It is not expected in this layer to affect the entities or external systems.

🔹 𝗜𝗻𝘁𝗲𝗿𝗳𝗮𝗰𝗲𝘀: The mechanisms by which the system communicates with external systems or users. Here we can have an MVC architecture of a GUI.

🔹 𝗖𝗼𝗻𝘁𝗿𝗼𝗹𝗹𝗲𝗿𝘀: The components responsible for managing the flow of data between the other layers of the system.

🔹 𝗣𝗿𝗲𝘀𝗲𝗻𝘁𝗲𝗿𝘀: The components responsible for presenting data to users or other systems.

🔹 𝗜𝗻𝗳𝗿𝗮𝘀𝘁𝗿𝘂𝗰𝘁𝘂𝗿𝗲: The components responsible for interacting with external systems or services, such as databases or APIs.

An 𝗮𝗽𝗽𝗹𝗶𝗰𝗮𝘁𝗶𝗼𝗻 𝘀𝘁𝗿𝘂𝗰𝘁𝘂𝗿𝗲 with Clean Architecture could look like, this for POS App:

📁 Source <br>
|__ 📁 Core <br> 
|____ 📁 Application <br>
|____ 📁 Domain <br>
|__ 📁 Infrastructure <br>
|____ 📁 Identity <br>
|____ 📁 Persistence <br>
|____ 📁 Shared <br>
|__ 📁 Api <br>
|__ 📁 ... <br>

In comparison to 𝗢𝗻𝗶𝗼𝗻 𝗔𝗿𝗰𝗵𝗶𝘁𝗲𝗰𝘁𝘂𝗿𝗲, Clean Architecture offers a clearer separation of concerns and a better comprehension of boundaries. They support similar ideals but with various levels, and they are close relatives. Clean architecture makes it crystal clear why each layer is necessary and what each one's roles are, which is why it is often referred to as 𝘀𝗰𝗿𝗲𝗮𝗺𝗶𝗻𝗴 𝗮𝗿𝗰𝗵𝗶𝘁𝗲𝗰𝘁𝘂𝗿𝗲.
