# MSA AI – Chatbot Project

## Problem Identification

In recent years, most of the developed economies need economy-wide actions to facilitate decarbonization and sustainable development as the world recovers from the COVID-19 global pandemic. Developed countries have been forced to rethink their development pathways in accordance with the goals of the Paris Agreement on climate change through long-term strategies.

Renewable energy investment has increased significantly in Australia over recent years, contributing to a continuing shift in the energy generation mix away from traditional fossil fuel sources.

It is evident that people will be curious and need ready resource which can answer their queries related to renewable energy investment. This project tries to resolve this issue by building a ChatBot service using Microsoft Azure Portal for AI services.

[![Investment in Renewable Energy](https://raw.githubusercontent.com/maheshhase/Microsoft-Azure-Projects/main/ChatBot/Images/image.jpeg "Investment in Renewable Energy")](http://https://raw.githubusercontent.com/maheshhase/Microsoft-Azure-Projects/main/ChatBot/Images/image.jpeg "Investment in Renewable Energy")


## Solution Design

I reasearched a lot of documentation related to Renewable Energy and found reports which gives a lot of information about investment in the renewable energy in Australia. However my solution design suffered from following setbacks

Size of the documents - I realised it later that we can upload only documents less than 1MB under free version
Text Analytics services do not have custom question answering mode under preview mode for free version
Further, artictecture design should be very simple so that gives prompt answer to user queries. I tried to manually review all chatbot answers related to article to avoid any wrong information. My entire project went through following phases :

Data Phase: This involved searching information which can answer queries related to renewable energy investment and yet brief enough to be less than 1MB. I choose URL approach over document, so that any updated information will be available to our user.
URL Link: Renewable Energy Investment in Australia



