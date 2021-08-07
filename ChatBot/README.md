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

- `Model Phase`: This involved 4 phases which are creating a resource group **RenewQnA**, followed by text analytics tool **RenewQnA** and QnA maker tool **RenewInvestment** using Microsoft Azure Portal. Final step involved creating a knowledge base using **qnamaker.ai** where database or resources were uploaded. This step will be discussed in detail in the next section i.e. Implementation of the Architecture.

- `Production Phase`: In this phase, I tried to develop **Web App Bot** but I could not utilise this feature due to limitations of free Azure version which did not allow Auto Creation of App ID and password.

[![Solution](https://raw.githubusercontent.com/maheshhase/Microsoft-Azure-Projects/main/Solution.jpeg "Solution")](https://raw.githubusercontent.com/maheshhase/Microsoft-Azure-Projects/main/Solution.jpeg "Solution")






