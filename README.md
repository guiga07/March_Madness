# Overview
Using .net and Visual Studio, we will construct a tournament tracker application that is fit to launch. The application uses Winforms, a class library, events, SQL database, text file data storage (in CSV format), custom events and more. This application can be used for arranging NCAA march madness tournament for example, which will be it's primary use.

# Big Picture Design

**Structure:** Windows Forms application and Class Libary

**Data:** SQL and Text File

**Users:** One at a time on one application

**Key Concepts:** Email, SQL, Custom Events, Error Handling, Interfaces, Random Ordering, Texting

# Mapping the Data
**Team**
- TeamMembers (List<Person>)
- TeamName (String)

**Person**
- FirstName (String)
- LastName (String)
- EmailAddress (String)
- CellphoneNumber (String)

**Tournament**
- TournamentName (String)
- EntryFee (Decimal)
- EnteredTeams (List<Team>)
- Prizes (List<Prize>)
- Rounds (List<List<Matchup>>)

**Prize**
- PlaceNumber (Int)
- PlaceName (String)
- PrizeAmount (Decimal)
- PrizePercentage (Double)

**Matchup**
- Entries (List<MatchupEntry>)
- Winner (Team)
- MatchupRound (int)

**MatchupEntry**
- TeamCompeting (Team)
- Score (Double)
- ParentMatchup (Matchup)

# User Interface Design
