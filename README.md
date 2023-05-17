# Booking-REST-API-Testing

## ***How to run this project***
- Clone this project
- Open with Postman / Command Shell
- Run Command:  
```console 
newman run Booking.postman_collection.json -e Booking-en.postman_environment.json 
```
- Run Command for Report: 
```console 
newman run Booking.postman_collection.json -e Booking-en.postman_environment.json -r cli,htmlextra
```

## ***Technology used***
- Postman
- Newman

## ***Prerequisite***
- Jdk
- Node Js
- Newman
- Html Report Library

## ***Newman and Report Installation Process***
- Newman Install Command:
```console
npm install -g newman
```
- Newman Html Report Install Command:
```console
npm install -g newman-reporter-htmlextra
```

## ***API Documentation***
- https://documenter.getpostman.com/view/27187339/2s93eVWZDJ

## Test case list
1. ### ***Create Booking***
	> In this section we created dataset using the dynamic random variables.

2. ### ***Get Booking***
	> In this section we tested wether we can get the details of the particular searched id which we got in the create booking section's response and also validated the following field values:
 	1. > First Name
 	2. > Last Name
 	3. > Total Price
 	4. > Deposit Paid
 	5. > Check In
 	6. > Check Out
 	7. > Additional Needs

3. ### ***Create Token***
  > In this section we generated a token that'll be needed to update the booking, partially update the booking and delete the booking.
  
4. ### ***Update Booking***
	> In this section we updated the following field values:
 	1. > First Name
 	2. > Last Name
 	3. > Total Price
 	4. > Check In
 	5. > Check Out
 	6. > Additional Needs
 	
5. ### ***Get Updated Booking***
	> In this section we tested wether the updated field values successfully added ot not and validated the following field values:
	1. > First Name
 	2. > Last Name
 	3. > Total Price
 	4. > Check In
 	5. > Check Out
 	6. > Additional Needs

6. ### ***Partial Update Booking***
	> In this section we just modified the following two field values:
	1. > First Name
 	2. > Last Name

7. ### ***Delete Booking***
	> In this section we deleted the information of the id that we called and successfully got the result.

## ***Newman Report Summary***
![1](https://github.com/Mahim-Hasan/Booking-REST-API-Testing/assets/77658882/d543e570-af34-4eaf-8f7c-becf4f3e202c)
![3](https://github.com/Mahim-Hasan/Booking-REST-API-Testing/assets/77658882/0c4ecfeb-8009-4545-a110-7c8b5e6745c0)