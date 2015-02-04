Medicost
========

OVERVIEW
--------
Medicost is a simple search engine made for people with high deductible insurance plans, where users can enter their location and requested service, and compare prospective prices from physician to physician within their area. The engine utilizes nearly 2 GBs of national data from [Medicare.gov](https://medicare.gov/) to compare rates (this is because most high deductible insurance plans have similar financial characteristics). Medicost was created at the MIT Hacking Medicine Hackathon in order to combat the rampant problem of price transparency in the medical world.

IMPLEMENTATION
--------------
We began by converting our CSV data to JSON, and then uploading them to our [Firebase](https://www.firebase.com/) database by using their REST API. From here, we would be able to do quick and specific searches directly through the database. Next, we made the front-end component for where users would actually input their general location and requested procedure. While we had a plethora of data to consult, we tried to keep the themes of procedures (Ex: Cardiology, Physical Therapy, etc.) down to the 100 most relevant subjects. In order to make the experience even easier, we added a fuzzy search component to the engine, so that we could ensure users would be able to find what they were looking for.

DISCLAIMER
----------
Medicost was created by [Sean Smith](https://github.com/sean-smith), [David Neary](https://github.com/davidneary), [Rahul Nath](https://github.com/rahul-nath), and I. All the data used was from the 2011 American Medical Association. 


Some useful tools I used:
https://github.com/firebase/firebase-import
https://github.com/shancarter/Mr-Data-Converter
