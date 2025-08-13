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









