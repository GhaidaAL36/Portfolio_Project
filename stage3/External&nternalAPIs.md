# External and Internal APIs

## External APIs

### OpenAI GPT API
The project uses the GPT API to power the core experience — explaining majors, generating tasks, evaluating user answers, and producing the results and feedback shown on the review page. It was chosen because it handles open-ended, conversational, and evaluative interactions well, which is exactly what Madar needs at every step.

---

## Internal APIs

### User API
Handles all user-related operations including registration, authentication, and profile management. Built to manage user sessions securely using JWT tokens, ensuring that only authenticated users can access the simulation features.

### Major API
Responsible for retrieving all available majors and their details including career paths and descriptions. Serves the Major Info Page by providing the data needed to display each major card to the user.

### Task API
Manages the generation and submission of tasks. When a user selects a major, it communicates with the AIEngine to generate a relevant task. Once the user submits their answer, this API forwards it for evaluation.

### Result API
Handles the storage and retrieval of user results after task evaluation. It calculates the final score and returns the feedback and recommendations displayed on the Review Page.

### AI API
The internal interface between the Backend and the OpenAI GPT API. It builds the prompts, sends them to GPT, and parses the responses before passing them back to the other APIs. It powers the core experience of explaining majors, generating tasks, and evaluating user answers.
