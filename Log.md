
## Systemideer:

- ”Kaffe-Vivino”

- App hvor chauffører kan beregne den hurtigste rute, når de skal levere cykler 

- Budget/+kvitteringsapp

- LinkedIn for kreative fag, hvor man kan vise sit arbejde frem for virksomheder og personer der er interesseret i at betale for ens arbejde. For (billed)kunstnere, fotografer, forfattere, programmører etc.

- Platform hvor virksomheder kan finde andre virksomheder, der kan leverer en ydelse eller et produkt virksomheden har brug for

- Webshop hvor der sælges smykker

- App hvor man kan scanne produkter i supermarkeder osv., og få informationer om indholdet af produkterne – for eksempel om det indeholder nødder, laktose etc., eller hvad hvor produktet er produceret og af hvem osv.

- Andet?


## Videreudvikling af systemideer:

### Videreudvikling af LinkedIn for kreative fag

- Et social medie, hvor man har en profil som enten kreativ fagperson (kunster, musiker, forfatter, multimediedesigner, programmør etc.) eller virksomhed
- Kreative fagpersoner kan på en god og professionel måde vise det de har lavet frem for virksomheder, der søger kreativt arbejde
- Mediet kan blive kombineret med en freelance marketplace, hvor freelancere kan sælge sig selv og virksomheder eller privatpersoner kan bestille arbejde
- Man skal evt. selv kunne designe/personaliggøre store dele af sin profil


## Funktionelle krav

### Brugere der ikke er logget ind (fremover: gæster):
- Hjemmesiden skal have en forside hvor man enten kan login eller gå til marketplace
- Brugeren kan browse "varer" på marketplace, men skal være logget ind for at kunne købe noget

### Brugere der er logget ind (fremover: brugere):
- Forsiden består af en header med 'profil', 'marketplace', 'feed', 'søgebar', 'chat', 'notifikationer', ' ???, som valgmuligheder og hvor body består af ens feed i midten 

- En bruger skal kunne lægge "et produkt"/"et værk" op på sin side, så andre brugere og gæster kan se produktet (defineret jf. bilag ??)
- En bruger skal kunne vælge at sætte et produkt til salg (på marketplace) (detaljer jf. bilag)
- En bruger skal kunne købe et produkt, der er sat til salg af en anden bruger
- En bruger skal kunne lave opslag, med tekst, billeder og/eller videoer, ligesom på facebook og linked in

- I søge-baren søge efter andre brugere, produkter, 
  
- Brugere skal kunne blive "venner" med hinanden/have forbindelse til hinanden via anmodninger
- Brugere, der har fået en venneanmodning, skal kunne afvise (anmoder notificeres om afvisning), acceptere eller ignorere (anmoder bliver ikke notificeret)
- Brugere, der har anmodet, bliver notificeret omkring den anmodets respons på anmodningen hvis personen ikke har valgt at ignorere anmodningen
  
- Brugere skal kunne sende private beskeder til dem de er venner med/er forbundet med
- Brugere skal kunne følge andre brugere (uden at være venner med dem), hvilket betyder de får notifikationer når den fulgte brugere laver opslag eller sætter noget til salg eller laver andre opdateringer
- Brugere skal kunne customize/designe deres profil i høj grad, så den bliver unik og personlig og fungerer som en erstatning for en personlig hjemmeside (defineret jf. bilag ??)


# Spørgsmål til Kim:

- Hvornår estimerer man sine user stories? Før eller efter sprint planning? 


# User stories

### USER STORY 1
- As a (logged in) user
- I want to be able to post a piece of work to my page
- so that I can share my work with potential buyers and/or companies that have an interest in hiring
___
### AC 1
- Given that I am on the upload work page
- when I have filled out the required boxes, so that the publish work button becomes active, and I have pressed 'publish work'
- then a message box saying "are you sure you want to publish this?" appears, and then, if I press 'Yes', my work is posted on my page so that me and other users will be able to see my posted work on my page and a page with a succes message appears and if I press "No", the message box
  dissapears and I can edit in the boxes 
  or
- then [some error handling: Appropriate error message]
___
___

### USER STORY 2
- As a user
- I want to be able to search for users and posted work
- so that I can see a user's profile and different user's work
___

### AC 2
- Given that I'm on the webpage
- when I have written something in the search bar
- then a list of user's and a list of posted work appears if any user's name or any posted work titles mathces what has been written in the search bar
  or
- then a message saying that no matches appears  

___
___

### USER STORY 3
- As a user
- I want to be able to customize my profile
- so that I can make my profile personal and unique and show of my creative abilities

___

### AC 3

- Given that I'm on the edit profile page
- when I have filled out the required boxes 
- then  
  if I have pressed 'Save changes' the changes are saved and my page appears with the changes  
  if I have pressed 'Preview' a preview appears where I can press 'Back to edit' or 'Save changes'  
  if I have left the edit profile page a message box appears saying "Are you sure want to leave without saving?"  

___
___

### USER STORY 4
- As a user
- I want to rate another user and be able to write a comment
- so that I can participate in a collected/common evaluation of the user 

___
### AC 4
- Given that I'm on a user's profile
- when I have pressed any number of stars between 1 and 5
- then a message box saying "Would you like to add a comment?" appears  and
- then if I press 'Yes' a text box appears and then if I press 'Save' the comment is saved in the db
  or then if I press 'X' or 'No' the box dissapears

___
___

### USER STORY 5
- As a user
- I want to see the comments connected to the ratings of a user
- so that I can get a more detalied picture of the quality of the user's work
   
___
### AC 5
- Given I am on a user's profile page
- when I press 'See comments/reviews'
- then a new page with a list of comments appears

___
___

### USER STORY 6
- As a user
- I want to be able to send direct, private messages to other users
- so that I can communicate privately with other users of interest 

___
### AC 6.1.1
- Given that I am on a users profile 
- When I have pressed 'Send message' on a users profile (to write a messsage to that user)
- Then a box appears with the receiver's name, a close [X] button, a box displaying messages sent,  
  a text box for writing messages and a 'Send' button

___
### AC 6.1.2
- Given that I am in my inbox (with a list of users I have a message thread with)
- When I press on a user  
- Then a box appears with the receiver's name, a close [X] button, a box displaying messages sent,  
  a text box for writing messages and a 'Send' button

___
### AC 6.2
- Given that I have written something in the text box
- When I press 'Send' (to send what I have written)   
- Then what I have written appears in the display of the text thread, and it appears in the receivers display  
  when she is logged in and opens our message thread   


___
___

### USER STORY 7
- As a user
- I want to be able to create a job posting
- so that I get job applications from artists that I can hire at my company or to do some work for me 

___
### AC 7.1
- Given that I am logged in
- When I press the 'Create job posting' button
- Then a job posting page appears with a formular for creating a job post.  
  The formular contains these boxes to fill out:
  1) Title (Limit of characters: 50)
  2) Job description (Limit of characters: 4800)
  3) Image or video (Format: mp4 or jpeg)
  
  If the limits in the parentheses are exceeded while writing, a message appears stating the limitations  
  If a wrong format for the image or video is chosen when uploading, a message appears stating the correct format
  

___
### AC 7.2
- Given that I am on the job posting page
- When I press 'Post job'
- Then one of several things happens:

  1) if there are no problems, a message appears saying "Confirm job posting". If confirmed a page with 
  the message "Success! Job posted. Go to job posts?" appears and all that have been entered in the formular is stored 
  in the database (and the job post appears in the list of job posts at the page given that someone 
  is on the job post page - could it be a user story by itself: As a user I want to see job posts?)  
  If not confirmed the message box dissappears and the user can edit the boxes in the formular.  

  3) if one or more boxes in the formular haven't been filled out, a message appears saying "Fill out all boxes"


___
___

### USER STORY 8
- As a (logged in) user
- I want to be able to post something (picture with text... etc)
- so that I can share my thoughts or achievements on the website to the public

___
### AC 8
- Given that I am on the post page
- When I have added a photo, video and/or text and pressed post
- Then the post will be uploaded and be public to all those on the feed
___
___

### USER STORY 9
- As a (logged in) user
- I want to be able to create a group
- so that I can gather likeminded people or discuss about a topic of interest with people within the same field

___
### AC 9.1
- Given that I am on the create group page
- When I filled out the required information for the creation of the group and pressed the create button
- Then a group will be created

___
### AC 9.2
- Given that I am creating a group
- When I selected the friends I want to add and press accept
- Then the selected friends will be added to the group upon it's creation
___
___

### USER STORY 10
- As a (logged in) user
- I want to be able to add friend(s)
- so that I can add people I enjoy communicating with or work well together with as friends on the website

___
### AC 10.1
- Given that I am on a persons profile page
- When I press on the add friend button on the profile
- Then a friend request will be recieved by the relevant person

___
### AC 10.2
- Given that I have sent a friend request
- When the relevant person has accepted the friend request
- Then the person and I have added each other as friends
   




  

 




