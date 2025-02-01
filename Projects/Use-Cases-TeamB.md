### Team: B - Lead Maitreyee
- Individual Use cases for final selection
1. Aditi Kapkar: Personalized AI Assistance Behavioral Therapy- (Rank - 1st)
2. Ishika Ramdham: Personal AI assistant for physically challenged individuals - (Rank - 5th)
3. Varenya Barve: AI powered resume screening and shortlisting system (Bias and Legal Issues) - (Rank - 4th)
4. Nikhil Khonde: Bookrecommender(Smart books recommendations and review app based on past purchases, new arrivals) - (Rank 2nd)
5. Maitreyee Warhadpande: Browser Extension for All Social media reviews AI sentiment analysis on <Product Reviews> (Search, View, Read Review, Add/remove to cart, Write Review) - (Rank - 3rd)

### Team B Final Use Case: Personalized AI Assistance Behavioral health Therapy - SoulSync
1. Short Name: (SSAI)

2. Description : The Personalized AI-Driven Behavioral Assistant is an advanced chatbot designed to revolutionize behavioral therapy by providing tailored emotional support, real-time mood tracking, guided therapeutic interventions, and seamless preparation for therapy sessions. This innovative tool is built to serve as a supportive companion for users.

The chatbot leverages state-of-the-art Natural Language Processing (NLP) techniques to deliver meaningful and empathetic interactions. Powered by BERT pre-trained word embeddings, the chatbot ensures deep contextual understanding of user inputs, enabling it to extract the intent and emotions behind the conversation effectively. Additionally, by using cosine similarity, the system performs high-accuracy similarity matching to retrieve the most relevant and verified responses from a vast database of advice and insights provided by psychologists worldwide.

3. Persona:
- Primary Users: Individuals with behavioral impairments seeking emotional support.  
- Secondary Users: Caregivers and behavior professionals who might use the chatbot as a supportive tool.

4. Painpoint:
- Limited access to affordable and reliable behvioral resources.  
- Hesitation or stigma around seeking help from professionals.  
- Difficulty understanding complex language or navigating traditional behvioral platforms.

5. Justification:
Developing an accessible behvioral chatbot addresses the increasing behvioral crisis, providing immediate, non-judgmental support to those who might otherwise hesitate to seek professional help. It bridges the gap between the demand for behvioral services and the availability of affordable solutions.

6. Benefits/Value:
- Offers 24/7 emotional support to users.  
- Promotes better behvioral management with tips and coping strategies.  
- Reduces the stigma of reaching out for help.  
- Provides a scalable and cost-effective solution for behvioral support.

7.Current State:
- Existing chatbots often lack accessibility for mentally impaired individuals or do not provide adequate support specific to their needs.  
- Limited conversational flow for behvioral scenarios.

8. Proposed State:
- A dedicated chatbot with simplified conversational flow, multi-language support, voice interaction, and a crisis escalation feature.  
- Integration with professional behvioral resources and helplines.

9. Solution:
- Build an AI-powered chatbot that uses NLP to understand user inputs and respond empathetically.  
- Develop conversation scripts tailored to behvioral support.  
- Implement accessibility features like text-to-speech, voice recognition, and visual cues.  
- Include an emergency protocol for connecting users to human assistance in crisis situations.

10. Technologies:
- NLP: For understanding conversations. 
- Frameworks: ML frameworks like TensorFlow or PyTorch for sentiment analysis. Microsoft Bot Framework for chatbot development.  
- Cloud: AWS, Google Cloud, or Azure for hosting and scalability.  
- Frontend: React or Flutter for mobile and web app integration.  
- APIs: Integration with behvioral resources or helplines.  
- Accessibility Tools: Text-to-speech APIs and voice recognition tools.

11. SIPOC
    Suppliers	- Psychologists & mental health experts (provide knowledge base)
              - AI/ML developers (build and train chatbot)
              - NLP API providers (Google Dialogflow, OpenAI, etc.)
              - Data sources (mental health articles, therapy resources)
              - End users (provide feedback for improvement)

  Inputs	- User messages (queries, emotional expressions)
          - Predefined mental health frameworks (CBT, mindfulness techniques)
          - NLP models for sentiment analysis & intent recognition
          - Data from previous conversations for personalization
          - Crisis intervention protocols

  Process	1. User interacts with chatbot via text/audio.
          2. NLP processes input, detects intent & sentiment.
          3. The chatbot selects an appropriate response (comforting messages, mindfulness exercises, coping strategies, or               crisis response).
          4. If needed, it provides resources (self-help guides, therapist contact suggestions).
          5. Logs interactions for future improvements while ensuring privacy.

  Outputs	- Personalized mental health support messages
          - Mood tracking insights
          - Guided therapy techniques (breathing exercises, journaling)
          - Crisis management responses (hotline suggestions, emergency alerts)
          - Analytics reports for chatbot improvement

  Customers	- Individuals struggling with mental health (students, professionals, general users)
            - Therapists (for therapy preparation & support)
            - Healthcare organizations (integrating AI in mental health services)

12. User Stories
User Story 1
Title: AI Chatbot for Nighttime Anxiety Support
As a person who struggles with nighttime anxiety,
I want a chatbot that can provide calming conversations and guided relaxation techniques,
So that I can manage my anxiety and sleep better.
Acceptance Criteria:
1.	Calming Conversations: The chatbot provides soothing and reassuring responses when I express stress before bed.
2.	Sleep Aid Techniques: It offers guided breathing exercises, bedtime stories, or meditation to help me relax.
3.	Gentle Notifications: It sends a soft reminder to practice relaxation techniques if I frequently report sleep difficulties.
4.	Journaling Support: It encourages me to write down my thoughts and worries to clear my mind before sleeping.
5.	Dark Mode & Soft Voice Feature: It has a visually calming interface with a text-to-speech option for a comforting experience.
Example Interaction:
•	User: "I can’t stop overthinking, and it’s making it hard to sleep."
•	Chatbot: "That sounds tough. Let’s try a simple grounding exercise: Name five things you can see, four things you can touch, three things you can hear, two things you can smell, and one thing you can taste. Take your time!"
________________________________________
User Story 2
Title: Motivational Mental Health Chatbot for Daily Encouragement
As a student facing academic pressure,
I want a chatbot that provides daily motivation and check-ins,
So that I can stay motivated and manage my stress levels better.
Acceptance Criteria:
1.	Daily Motivation Messages: The chatbot sends me positive quotes or affirmations every morning.
2.	Goal-Tracking Support: It helps me set and track small, achievable goals for the day.
3.	Encouraging Responses: When I feel discouraged, it offers uplifting messages and reminds me of my progress.
4.	Customizable Encouragement: I can personalize the type of motivation I want—whether it's study tips, productivity hacks, or self-care reminders.
5.	Reflection & Gratitude Prompts: It asks questions like "What’s one thing you’re proud of today?" to reinforce a positive mindset.
Example Interaction:
•	User: "I feel like I’m not making any progress in my studies."
•	Chatbot: "Progress isn’t always visible right away, but every small effort adds up! Think about where you were a month ago—you’ve come a long way. What’s one topic you understand better now?"
________________________________________
User Story 3
Title: AI Chatbot for Social Anxiety Support
As a person struggling with social anxiety,
I want a chatbot that helps me practice conversations and gain confidence in social situations,
So that I can feel less anxious when talking to people.
Acceptance Criteria:
1.	Simulated Conversations: The chatbot allows me to practice casual conversations to build confidence.
2.	Personalized Advice: It gives me strategies to manage anxiety in real-life social interactions.
3.	Breathing & Relaxation Techniques: It guides me through calming exercises before and after social interactions.
4.	Progress Tracker: It helps me track my comfort level over time in different social situations.
5.	Encouragement & Reinforcement: It reminds me that social skills improve with practice and provides positive reinforcement.
Example Interaction:
•	User: "I have to give a presentation tomorrow, and I’m really nervous."
•	Chatbot: "I understand! Let’s do a quick confidence boost. Imagine your future self-finishing the presentation successfully—how does that feel? Want me to guide you through a deep breathing exercise?"
________________________________________
User Story 4
Title: AI-Powered Mental Health Chatbot for Emotional Support
As a college student experiencing stress and loneliness,
I want an AI-driven chatbot that provides emotional support, mindfulness exercises, and positive reinforcement,
So that I can manage my stress, feel emotionally supported, and develop healthier coping mechanisms.
Acceptance Criteria:
1.	Emotional Check-ins: The chatbot prompts me daily to share how I’m feeling and tracks my emotional patterns over time.
2.	Mindfulness & Coping Exercises: It suggests relaxation techniques, guided meditations, and positive affirmations based on my mood.
3.	Conversational Support: It engages in empathetic conversations, offering comforting and reassuring responses when I feel overwhelmed.
4.	Crisis Response: If I indicate severe distress, it provides immediate self-help resources and suggests contacting a mental health professional.
5.	Privacy & Security: My conversations and emotional data are stored securely and kept confidential.
Example Interaction:
•	User: "I feel really alone and unmotivated today."
•	Chatbot: "I'm here for you. It sounds like you're having a tough day. Would you like to talk about it or try a small activity to lift your mood?"
•	User: "Maybe an activity would help."
•	Chatbot: "Let's try a gratitude exercise. Can you think of one small thing that made you smile recently? It can be anything—like a good meal or a kind word from a friend."
________________________________________
User Story: 5
Title: Enhancing Emotional Well-being with the AI-Driven Mental Health Assistant  
As a young professional experiencing anxiety,  
I want a personalized and empathetic mental health assistant,  
So that I can manage my emotions, track my mood, and prepare for therapy sessions effectively.  

Acceptance Criteria:
1. Mood Tracking: The assistant allows me to log my emotions daily and provides insights into patterns over time.  
2. Guided Interventions: It offers personalized therapeutic exercises like breathing techniques or journaling prompts tailored to my mood and stress levels.  
3. Real-Time Support: It responds empathetically and provides helpful advice when I share feelings of anxiety or distress.  
4. Therapy Preparation: It helps me organize my thoughts and prepare questions to make my professional therapy sessions more productive.  
5. Confidentiality: It ensures my data is secure and private.  

Example Interaction:
- User: "I'm feeling overwhelmed and stressed about work."  
- Assistant: "I'm here for you. It sounds like you're under a lot of pressure. Would you like to try a short breathing exercise to calm down or talk through what's making you feel overwhelmed?"  
- User: "A breathing exercise sounds good."  
- Assistant: "Great. Let's try this: Inhale deeply for four seconds, hold for four seconds, and exhale slowly for six seconds. Repeat this five times. Let me know how you feel afterward."



