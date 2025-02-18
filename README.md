# IPL Schedule Optimization

## 📌 Project Overview
This project aims to optimize the **IPL 2024** schedule to **minimize travel and accommodation costs** for teams. The optimization involves selecting the best airline and hotel partners while considering the total tournament duration, rest days, and dynamic pricing of flights and hotels.

## 🏆 Objectives
- Reduce **travel and accommodation costs** by optimizing scheduling.
- Ensure **teams have sufficient rest days** while maintaining a fair match distribution.
- Minimize **worst-case travel distances** by selecting centralized venues for final matches.

## 🚀 Assumptions
- Players travel to the match venue one day before and rest for a day post-match.
- Hotel stays range from **3 to 4 nights** per team.
- Flight and hotel pricing is dynamic per day but remains static for a single day.
- Airline and hotel partners are available in **all cities**.
- **Weather conditions** do not impact scheduling.

## 📊 Decision Variables
- **Team Travel (Yt,i,j,a,d)** → Represents a team's flight between venues.
- **Match Scheduling (Xt,v,d)** → Defines which teams play at a specific venue on a given day.
- **Flight Cost (Ci,j,a,d)** → Cost for a team's travel between venues.
- **Hotel Cost (Hh,v,d)** → Accommodation cost per venue and day.

## 🏁 Optimization Approach
1. **Minimizing travel & hotel costs** through an objective function.
2. **Constraints applied:**
   - Each team travels between **8 to 14 times**.
   - Maximum **4 flights per day**.
   - Travel occurs only one day before a match.

## 📍 Phase-2: Venue Optimization
- Using **center of mass calculation**, we determine an optimal **central stadium** to host the last **4 matches**.
- **Hotel costs influence venue selection**, with preference given to cost-effective locations.

## 📂 Data Sources
- **Flight Costs** → Scraped fro
m **ixigo.com**.
- **Hotel Costs** → Extracted from **Booking.com**.
- **Venue Selection** → Uses a **map projection** of India.


