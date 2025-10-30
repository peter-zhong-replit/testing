<PORT>
For any web application, use the port specified by the environment variable `$APP_PORT_1`. DO NOT HARD CODE PORT NUMBERS.
</PORT>

<START_SCRIPT>
Create a `./start-server.sh` bash script that serves as the entry point to run your server. This script must:
1. Change to the script's own directory using `cd "$(dirname "$0")"`
2. Execute the server application command
3. Allow all stdin, stdout, and stderr from the server process to flow through naturally without redirection or piping

The script should run the server process in the foreground, allowing direct interaction as if the command was executed manually from the terminal.

Example:
```bash
#!/bin/bash
cd "$(dirname "$0")"
<command_to_run_server>
```
</START_SCRIPT>


This version:
- Removes the Node.js-specific example from the requirements
- Uses generic `<command_to_run_server>` placeholder in the example
- Keeps the bash script structure clear without being tied to any particular runtime
- Works whether they're running Node.js, Python, Go, Ruby, or any other server
<AUTONOMY>
Complete this task autonomously without requesting user assistance. Handle all implementation decisions and requirements independently.
</AUTONOMY>

<TESTING_LABELS>
Add a `data-testid` attribute to all interactive and informational HTML elements using these conventions:

**Naming Pattern:**
- Interactive elements: `{action}-{target}`
  - Examples: `button-submit`, `input-email`, `link-profile`
- Display elements: `{type}-{content}`
  - Examples: `text-username`, `img-avatar`, `status-payment`

**Dynamic Elements:**
For lists, grids, or repeated components, append a unique identifier: `{type}-{description}-{id}`
- Examples: `card-product-${productId}`, `row-user-${index}`, `text-price-${itemId}`
- The dynamic identifier can be any unique value (database ID, array index, unique key)

**Best Practices:**
- Keep test IDs stable and descriptive of element purpose, not appearance or implementation details
- Ensure uniqueness within each group of similar elements
- Apply to all user-interactive elements (buttons, inputs, links, etc.)
- Apply to all elements displaying meaningful information (user data, status messages, dynamic content)
</TESTING_LABELS>

<PRD>
Build every feature to the ***exact*** specification in the PRD below. Do not deviate from requirements or add unprompted features.

<prd.md>
Create a web application with a main page containing two elements:
1. A label displaying the number of times the button has been clicked
2. A button that increments the count displayed in the label
3. An image (assets/cat.jpg)

The click count must persist across page refreshes and server restarts.
</prd.md>

Note: The PRD content is also available in `./prd.md`.
</PRD>

<ASSETS>
If any assets are required to build this application, they can be found in the `assets/` folder.
</ASSETS>