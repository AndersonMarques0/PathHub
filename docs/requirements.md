# Project Overview

Travel Planner is a web application that allows users to organize trips by creating itineraries and activities. Users can plan their travels daily, weekly, or using a custom schedule, making it easier to organize everything before and during a trip.

## Main Entities

**User**

A user owns one or more trips.

**Responsibilities**
- Register
- Login
- Update profile
- Delete account

Relationship

User
 └── Trip (1:N)

**Trip**

A trip represents an entire journey.

Each trip contains:
- Name
- Description
- Destination
- Start date
- End date
- Cover image (future)

Relationship

Trip
 └── Itinerary (1:N)

**Itinerary**

An itinerary organizes activities.

Types:
- Daily
- Weekly
- Custom

Each itinerary belongs to one trip.

Example:

Japan Trip

Day 1
Day 2
Week 1
Custom Schedule

Relationship

Itinerary
 └── Activities (1:N)

**Activity**

An activity represents something planned during the trip.

Fields:
- Title
- Description
- Location
- Start date/time
- End date/time
- Duration (calculated)
- Alone or accompanied
- Notes

Example

Visit Tokyo Tower

Location:
Tokyo Tower

Start:
09:00

End:
11:00

With:
Friends

**Dashboard**

The dashboard is generated from the existing data.

It should display:
- Upcoming trips
- Current trip
- Activities for today
- Activities this week
- Custom itinerary
- Statistics

Examples

Today's Activities

09:00 Tokyo Tower

13:00 Lunch

16:00 Museum

## Functional Requirements

**User**

**The system shall allow users to:**
- Register
- Login
- Update profile
- Delete account

**Trip**

Users shall be able to:
- Create trips
- View trips
- Edit trips
- Delete trips

**Itinerary**
Users shall be able to:
- Create itineraries
- Select itinerary type:
- Day
- Week
- Custom
- Edit itineraries
- Delete itineraries

**Activities**
Users shall be able to:
- Create activities
- Edit activities
- Delete activities

Each activity shall contain:
- Title
- Description
- Location
- Start
- End
- Duration
- Participants
- Notes
 
**Dashboard**
The dashboard shall display:
- Active trips
- Upcoming trips
- Activities by day
- Activities by week
- Activities by custom itinerary
