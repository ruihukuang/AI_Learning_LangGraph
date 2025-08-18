# AI_Learning_LangGraph    

## lab 1    
Context   

Integrate LangGraph with LLMs and use a gradio UI to create a chatbox shown in the screenshot below.  

A question is asked but an accurate answer is not provided.  

<img width="974" height="569" alt="image" src="https://github.com/user-attachments/assets/afafa65e-bf11-48e9-b0fb-0399d739d8a2" />  

## lab 2  
Context  

- Step 1: Use a LangChain wrapper class for converting functions into Tools.   
Convert a Serper API function into a tool to search content from websites with google search API.   
Convert a push function into a tool to send a notification to a pushover app on my phone.
  
- Step 2: Integrate the tools created from step 1 with LangGraphs and LLMs to create a chatbox shown in the screenshot below.   
The same question from the lab 1 is asked but the chatbox could answer it more accurately this time. The chatbox could send a notification to a pushover app as requested. But it could not keep memory from previous conversations/interactions. Even though I told the chatbox my name previously, it still could not recall my name.      
<img width="1616" height="884" alt="image" src="https://github.com/user-attachments/assets/e451446d-13c9-40c3-b1f7-656e687c04aa" />       
<img width="1244" height="611" alt="image" src="https://github.com/user-attachments/assets/b96bba05-0ac5-4c5c-a7b8-5a03a718b3ab" />  
 
- Step 3 : Add a memory server object into step 2 with different thread id for different individual chats. In this case, it could recall content from previous conversations/interactions for example a name or an instruction of sending a notification to my phone.   
Screenshots below show a chatbox could remember my name after I told it and also could send the same notification without telling it the content.    
<img width="1529" height="710" alt="image" src="https://github.com/user-attachments/assets/7c87becf-d86f-4ef8-a870-c7e7973ce903" />  
<img width="1705" height="1019" alt="image" src="https://github.com/user-attachments/assets/d4d2380c-bfc5-4592-9820-8da5374ce6ac" />

- Step 4 : Save memory into files rather than just adding a memory server object. In this case, a chatbox could use info from memory files to start conversations but could be updated based on requests during conversations.  
A screenshot below show a chatbox starts calling me another name from memory files but could call me a right name after I correct it.   
<img width="1588" height="844" alt="image" src="https://github.com/user-attachments/assets/47d0477a-7167-44f4-a4ce-18de89a0f2df" />  

All the conversations/interactions generated from LangGraphs are monitored in the Langsmith shown in the screenshot below.  
<img width="2964" height="1488" alt="image" src="https://github.com/user-attachments/assets/d5640cf5-b0eb-423f-a6b9-92e1ec60d141" />  

## lab 3  

Context  
Use LangGraph to create a workflow. This workflow enables a chatbox to trigger tools if needed. There are 2 tools. One tool is to extract text from web browsers using Playwright and Node.js from LangChain. The other one is to send a push notification to a Pushover app to my phone.  

Use LangGraph to create a workflow:      
<img width="236" height="264" alt="image" src="https://github.com/user-attachments/assets/deaaad8f-1f97-4012-ac2d-995089864c78" />  

Trigger to open web browsers using Playwright and Node.js:  
<img width="1278" height="371" alt="image" src="https://github.com/user-attachments/assets/fc6f25dd-9486-4994-a961-59049acb312f" />  

Trigger to send a push notification to a Pushover app to my phone in the chatbox:  
<img width="1003" height="524" alt="image" src="https://github.com/user-attachments/assets/6ff930a3-6c3b-4872-a2fb-1f6ab057a1f8" />   

## lab 4   

Context  
Create a LangGraph to start a workflow. This workflow adds evaluators on the top of the workflow from lab 3. It requires a chatbox to enter a question and criteria. This criteria is used by evaluators to provide the feedback on the answer.  

Use LangGraph to create a workflow:  
<img width="287" height="377" alt="image" src="https://github.com/user-attachments/assets/debab61d-44bc-4835-bf43-b030f98125a6" /> 

Trigger to open web browsers using Playwright and Node.js:   
<img width="1270" height="429" alt="image" src="https://github.com/user-attachments/assets/f1593ded-3135-49f2-92c9-988769911d71" />    

Provide an answer and evaluator feedback on the answer in the chatbox:   
<img width="1033" height="545" alt="image" src="https://github.com/user-attachments/assets/3b4d381f-e6f1-4563-b59f-3a20b9b8d443" />  

## app folder   

Context  
An app is created to include a workflow from lab 4 and also to add other tools using Langchain. These tools include using a file system to save responses from the workflow, using Wikipedia to immprove search and using Python REPL for debugging.  

The screenshots below shows an app launched locally with a request from a user and responses for using tools. The tools are used to save responses and to send a notification to a Pushover app on my phone.  

<img width="1305" height="679" alt="image" src="https://github.com/user-attachments/assets/eb491ed0-b356-4e97-8cbb-0609ad0a295c" /> 

<img width="1301" height="675" alt="image" src="https://github.com/user-attachments/assets/54b18bbf-2c77-45a4-bd17-6e3991747fdb" />  


The app also uses tools to search webs using web browsers, extract content from webs, and search Wikipedia etc. The usage could be found in LangSmith. The screenshot below shows some usages for these tools.   
<img width="1297" height="700" alt="image" src="https://github.com/user-attachments/assets/f84ac2bf-cc85-48be-891b-11357f0ebdab" />  









