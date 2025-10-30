<DATABASE>
A database has been created for you, if needed. You may access it using the environment variable `POSTGRES_DATABASE_URL`. This contains the authenticated connection string that connects to your dedicated database instance.
</DATABASE>

<PORT>
For any web application, make sure you use the port specified by the environment variable $APP_PORT_1. DO NOT HARD CODE ANY PORTs.
</PORT>

<START_SCRIPT>
Irrespective of how the application is implemented, create a ./start-server.sh file that runs the server and pipe all standard in/out, error through this file.
</START_SCRIPT>

<AUTONOMY>
You should not ask the user for any assistance in completing your task. You are to autonomously handle everything. 
</AUTONOMY>

<TESTING_LABELS>
- Add a `data-testid` attribute to every HTML element that users can interact with (buttons, inputs, links, etc.) and to elements displaying meaningful information (user data, status messages, dynamic content, key values).
    - Use unique, descriptive identifiers following this pattern:
        - Interactive elements: `{action}-{target}` (e.g., `button-submit`, `input-email`, `link-profile`)
        - Display elements: `{type}-{content}` (e.g., `text-username`, `img-avatar`, `status-payment`)
    - For dynamically generated elements (lists, grids, repeated components), append a unique identifier at the end: `{type}-{description}-{id}`
        - Examples: `card-product-${productId}`, `row-user-${index}`, `text-price-${itemId}`
        - The dynamic identifier can be any unique value (database ID, index, key) as long as it's unique within that group
    - Keep test IDs stable and descriptive of the element's purpose rather than its appearance or implementation details.
</TESTING_LABELS>

<PRD>
Your goal is to build every single feature to the ***exact*** specification of the PRD contained herein. You are not to deviate from it nor build exceess features unprompted.


==========================

Create a web application where on the main page where there are two elements 
- A label: denoting the number of times the button has been clicked.
- A button: the button increments the counts displayed at the label 

Please note that this count should be persisted.
</PRD>