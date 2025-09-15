# Groq API Assignment: Conversation Management & Classification
##  Objective
Implement two core tasks using Groq APIs with OpenAI SDK compatibility:
1. **Conversation Management** with summarization and truncation
2. **JSON Schema Classification** using function calling for information extraction

##  Requirements Compliance
-  **No frameworks** - Only standard Python + OpenAI client
-  **Groq API integration** - OpenAI-compatible SDK
-  **Colab notebook** - Clean code with visible outputs
-  **API key included** - Ready for testing


##  Task Implementation

### Task 1: Conversation Management
- **ConversationManager class** - Stateful conversation handling
- **Memory management** - Summarization every k-th run
- **Truncation options** - By message count or character limit
- **Groq API integration** - Uses llama-3.1-8b-instant for summarization

### Task 2: JSON Schema Classification
- **5-field extraction** - name, email, phone, location, age
- **Function calling** - Uses llama-3.3-70b-versatile model
- **Schema validation** - Required fields and type checking
- **3 sample demonstrations** - Complete with validation results

## Project Structure
```
groq-assignment/
├── conversation_management.ipynb    # Main implementation
├── groq_assignment_flow.txt        # Flow diagram
└── README.md                       # This file
```

##  Key Features
- **Conversation history** with intelligent summarization
- **Context management** with configurable limits
- **Structured extraction** using JSON schema validation
- **Error handling** with graceful fallbacks
- **Clean demonstrations** with visible outputs

##  Expected Outputs

### Task 1 Results
- Conversation history maintained across multiple turns
- Summarization triggered every 3rd run
- Truncation working for both message count and character limits

### Task 2 Results
- Information extracted from 3 sample chats
- JSON validation showing required fields (name, email)
- Structured output with validation status

##  Demo Samples
```python
# Sample Chat 1
"Hi, my name is John Smith. I'm 25 years old and live in New York City. 
My email address is john.smith@example.com and you can reach me at 555-123-4567."

# Expected Output
{
  "name": "John Smith",
  "email": "john.smith@example.com", 
  "phone": "555-123-4567",
  "location": "New York City",
  "age": 25
}
```
