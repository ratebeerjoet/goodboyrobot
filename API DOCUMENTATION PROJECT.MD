API DOCUMENTATION PROJECT

EVALUATION CRITERIA
- How easy would it be for an outside developer to understand the API instructions? 
- How feasible is the technology required for the API to work? 

EVALUATION 
1. ALMANAC 
- This API would be very easy for a developer to understand. All they would need to do is input straightforward data like location, activity and time, and the API will give them straightforward data back. Additionally all the data needed, like weather, tides, or local news alerts, are already public and easily accessible information. For these reasons, I believe Almanac would make the simpelest documentation project. 
2. STARROUTE 
- uilding the actual system would be very easy because the  Gaia database already has the information we need: they’ve mapped and cataloged over a billion stars and their positions. All StarRoute would need to do is use that raw data to calculate things like a space ship's travel time between two set points. The issues are the 3d modelling and the specialized knowledge required of the developer. Designing a scaleable, interactive, 3d star map from the Gaia data would be a huge project, as Claude put it ‘more of a graphic design project than an api one.’ Additionally, in order to properly use the API, a developer would likely have to be familiar with astronomy concepts like parallax, and time dilation and know how to understand galactic coordinates. 

3. TACTICA 
- Although the interactions should be straightforward for a developer (it’s just ‘send a game state, then get back a recommended move plus reasoning’), in my opinion, the technology required for this API is unfeasible. First, extrapolating the board state of a table top game from a photograph is extremely challenging. Determining which models are which from hundreds of options and accounting for various paint schemes and kitbashing (model customization) would be difficult, as would be determining exact distances and lines of sight without a standardized perspective. Second, keeping up to date with large rules sets that are constantly being updated, expanded and errata'd would require continuous work, unless there was a way to have the program automatically update itself. Many of these rules, such as individual unit stats for warhammer models, are also paywalled in physical book releases and not freely available online from legal sources. 

ARGUMENT AGAINST ALMANAC
- The most difficult part of this project will be getting the system to determine what information is relevant to a given request. Pulling up raw data about a place will probably be straightforward, but then it will have to sort it. If someone plugs in that they’re going kayaking in the Gorge at 2:00pm, the API will have to know how to sort important things: tides and weather, from non-relevant things like, say, which local wild berries are safe to eat. However, I think this challenge is much more simple and approachable than building a full 3d interactive star map, or trying to get access to every paywalled warmhammer ruleset. Therefore, I still believe Almanac will make the simplest documentation project. 

