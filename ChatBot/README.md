# MSA AI – Chatbot Project

## Problem Identification

In recent years, most of the developed economies need economy-wide actions to facilitate decarbonization and sustainable development as the world recovers from the COVID-19 global pandemic. Developed countries have been forced to rethink their development pathways in accordance with the goals of the Paris Agreement on climate change through long-term strategies.

Renewable energy investment has increased significantly in Australia over recent years, contributing to a continuing shift in the energy generation mix away from traditional fossil fuel sources.

It is evident that people will be curious and need ready resource which can answer their queries related to renewable energy investment. This project tries to resolve this issue by building a ChatBot service using Microsoft Azure Portal for AI services.

[![Investment in Renewable Energy](https://raw.githubusercontent.com/maheshhase/Microsoft-Azure-Projects/main/ChatBot/Images/image.jpeg "Investment in Renewable Energy")](http://https://raw.githubusercontent.com/maheshhase/Microsoft-Azure-Projects/main/ChatBot/Images/image.jpeg "Investment in Renewable Energy")


## Solution Design

I reasearched a lot of documentation related to Renewable Energy and found reports which gives a lot of information about investment in the renewable energy in Australia. However my solution design suffered from following setbacks
1. Size of the documents - I realised it later that we can upload only documents less than 1MB under free version
2. Text Analytics services do not have custom question answering mode under preview mode for free version

Further, artictecture design should be very simple so that gives prompt answer to user queries. I tried to manually review all chatbot answers related to article to avoid any wrong information.  My entire project went through following phases :

- `Data Phase`: This involved searching information which can answer queries related to renewable energy investment and yet brief enough to be less than 1MB for free version. I choose URL approach over document, so that any updated information will be available to our user.
URL Link: [Renewable Energy Investment in Australia](https://www.rba.gov.au/publications/bulletin/2020/mar/renewable-energy-investment-in-australia.html "Renewable Energy Investment in Australia")

- `Model Phase`: This involved 4 phases which are creating a resource group **RenewQnA**, followed by text analytics tool **RenewQnA** and QnA maker tool **RenewInvestment** using Microsoft Azure Portal. Final step involved creating a knowledge base using **qnamaker.ai** where database or resources were uploaded. 

- `Production Phase`: In this phase, I tried to develop **Web App Bot** but I could not utilise this feature due to limitations of free Azure version which did not allow Auto Creation of App ID and password. Having said this limitation, this project is certainly **Scalable** and **Extensible** with paid version of the Microsoft Azure Services.

These steps will be discussed in detail in the next section i.e. Implementation of the Architecture.

[![Solution](https://raw.githubusercontent.com/maheshhase/Microsoft-Azure-Projects/main/Solution.jpeg "Solution")](https://raw.githubusercontent.com/maheshhase/Microsoft-Azure-Projects/main/Solution.jpeg "Solution")

## Implementation of Architecture:

1.  `Setting up Microsoft Azure Portal`
	- As a newcomer, I started with basic steps of implementation which is creation of student account for Microsoft Azure Portal.
	- After multiple iterations, I could setup a **Resource Group** for ChatBot Project. I was trying to intergrate **Text Analytics services**, but could not do so due to limitations of free tier account.
	- FInally, I created **QnA Maker** using same resource group to make a ChatBot.
	
2. `Data Phase`
	- I searched a lot of resources for Renewable Energy sources of Australia as well as **Reserve Bank of Australia** to get recent investment in the Renewable Energy.
	- Due to limitations of free tier account, I could only upload resources upto 1MB. I realised this much later after researching a lot of useful articles for chatbot. Hence, this phase consumed a lot of time due to technical limitations of free tier account.
	
3. `Model Phase`
	- This was the most interesting phase of the project. I used **qnamaker.ai** to create a knowledge base for chatbot. I uploaded resource from **Reserve Bank of Australia**  which talks about latest trends of the investment in the Renewable Energy sector of Australia.
	- I tried to use **preview mode** to make ChatBot more interactive using text analytics services. However, this did not enable feature to try custom question answering while Populating the database.
	- I used **Professional** persona to answer queries of students, researchers and industry people while creating knowledge base.
	
4. `Train Phase`
	- I have to **manually edit responses** to queries as they capture certain irrelevant responses such as text version of images and tables, references, introduction etc.
	- Further, I included **more questions for each response** depending on keywords in the response for better functionality.

5. `Test and Population Phase`
	- I tested the QnA maker for certain questions multiple times till I get satisfactory response. 
	- Responses were designed to provide detailed response to user so that they get maximum information related to topic.
	- Further, professional persona took care of general questions being asked by user.
	
6. `Production Phase`
	- I tried to create **Web App Bot** by creating new app name and bot handle linked to same resource group.
	- However, due to limitations of the free tier service, I could not auto create App ID and Password. Hence, I will update complete the step once free tier service is upgraded to generate auto creation of App ID and Password.





