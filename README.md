# MongoDB-Showcase

This GitHub repository has been created as a part of a university project and contains the code for data modeling and optimization.

The objective of the project is to develop a data model for a specific application and optimize it to meet the requirements of the application. The code is divided into different sections:

1. ``Data Modeling``: This section contains the code for creating the data model, including entities, relationships, and attributes. The code is designed to be easily extendable in case the requirements for the data model change.

2. ``Data Optimization``: This section provides the code for optimizing the data model. Different optimization techniques are employed to improve the performance of the application, such as indexing, partitioning, and materialized views.

3. ``Sample Application``: The code for a sample application that uses the developed data model is also included in this repository. It is a web application that uses the developed data model.



When making changes to the data structure, we started with several relevant assumptions in mind:

First, we wanted to optimize the display of the homepage for the property. This means that we focused on ensuring that the most relevant information was easily accessible and displayed in a user-friendly manner.
Second, we identified errors in the data that needed to be corrected or removed. This included removing duplicates (such as _copy1, _copy2) and correcting incorrect transaction dates. We also considered the impact of changing the data structure on the existing code and tried to adapt it where necessary. In some cases, we opted for sub-optimal solutions to avoid breaking the existing code.
Third, we recognized that some changes in the data structure would require updating the code. For example, the way scores were stored needed to be changed because there was no way to incorporate a new score. We had no way of knowing if a rating of 4 was the average of 100 people or just one person, making it difficult to update the score when a new rating was added.
Fourth, we created indexes only where we found it to be extremely relevant. We were aware that indexes come at a cost, especially in terms of update operations and storage space, so we tried to be selective in their use.
Finally, we made some of the commands idempotent to ensure that running them twice would not impact the data structure. This was done to reduce the risk of unintended consequences and make it easier to revert changes if necessary.

