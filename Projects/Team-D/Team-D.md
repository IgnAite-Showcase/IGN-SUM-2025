Team: D - Lead (Atharwa)
- Individual Use cases for final selection
1. Yachana Mahant: AI Assistant for Farmers to take advantage of Government Schemes in local Language
2. Atharva Jibhakate: Personalized Travel Itinerary Generator (Door/End - Door/End)(Rank1)
3. Prajwal Potfode: SecureVision - Automated Security Identitity Detection for Criminal Background Suspects.
4. Purva Thote: Portfolio Tracker(Rank2)
Description: A web app for tracking personal investments (stocks, crypto, etc.).

### Team D Final Use Case:  Personalized Travel Itinerary Generator (Door/End - Door/End)

- Short Name: SmartJourney

- Description:
1. SmartJourney is an AI-powered platform that creates personalized, end-to-end travel itineraries.
2. It considers user preferences, budgets, and constraints to recommend optimized travel plans,
3. Including transportation, accommodations, activities, and local experiences and buffer time.

- Persona:
1. Primary Users: Personalized travel planning, for individuals or families, and corporate travelers seeking tailored trip planning solutions.
2. Secondary Users: Useful for travel agencies and businesses offering customized travel services.

- Painpoints:
1. Time-consuming process to plan trips, comparing multiple platforms for bookings and activities.
2. Difficulty in finding personalized recommendations for unique preferences.
3. Lack of real-time adjustments based on unforeseen changes like delays or weather or changes in priorities.
4. Overwhelming options leading to indecision and suboptimal plans.

- Justification:
Travelers seek streamlined, stress-free planning and unique experiences, yet traditional platforms require extensive manual effort. SmartJourney leverages AI to automate and personalize the planning process, enhancing user satisfaction and travel efficiency.

- Benefits/Value:

Personalization: Curated itineraries tailored to user preferences and budgets.
Efficiency: Minimized planning time by consolidating travel, lodging, and activities in one platform.
Real-Time Adjustments: Dynamic updates for weather, delays, or preference changes.
Cost Savings: Optimize costs with AI-driven recommendations and deals.
Convenience: Door-to-door service covering every step of the journey.

-Current State:

Travelers rely on multiple platforms (Google Maps, Booking.com, Expedia, etc.) for research and bookings.
Manual coordination of travel schedules and activities is common.
Limited integration between planning and real-time updates.

-Proposed State:

Unified AI-powered platform for planning, booking, and real-time updates.
Integrated transportation, lodging, and activity recommendations with a seamless user experience.
AI-powered chatbot for personalized guidance and adjustments on the go.

-Solution: Chatbot (Generate Iternary, Adjust Iternary)
AI Assistance: Intelligent itinerary generation based on user preferences, budget, and real-time data.
Real-Time Adaptability: Automatic updates for weather changes, delays, or cancellations.
Integrated Booking: Direct bookings for transport, hotels, and activities from the platform.
User Profiles: Save preferences and past trips for tailored recommendations.
Collaboration Features: Group trip planning with shared itineraries and budget tracking.
Responsive Design: Easy access via responsive web and mobile applications.

-Technologies:
Browser-Based Frontend: React, TypeScript, Tailwind CSS, Next.js
Backend: Node.js, Express
AI/ML Models: GPT models for personalized suggestions and NLP-based user interaction
Databases: MongoDB for user data, preferences, and itinerary storage
APIs: Integrations with Google Maps, OpenWeather, Booking.com, and other travel-related APIs
Collaboration Tools: Real-time updates via WebSockets or WebRTC
Payment Gateways: Integration with Stripe or PayPal for seamless transactions

- Use Case Methodology: SIPOC
1. Supplier: Traveler  (Context: My current location, Todays Date)
2. Input: Prompt- I would like to have vacation at Goa on MM-DD-YYYY (Chat GPT) and other details eg: budget, interests, etc
3. Process: State T0 JSON(Current(Nagpur) -[Parameters]-> Destination(Goa) -[Parameters]-> Current(Nagpur))
4. Output:  State T1 JSON(Current(Nagpur) -[Parameters]-> Destination(Goa) -[Parameters]-> Current(Nagpur))
5. Customer: Traveler (gets iternrary after finalizing) 

