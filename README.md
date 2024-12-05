<img src="https://assets.publish.postman.com/og-image?heading=COLLECTION&entityName=Natours%20API%27S&entityType=collection-documentation&imageUrl=https%3A%2F%2Fres.cloudinary.com%2Fpostman%2Fimage%2Fupload%2Ft_user_profile_300%2Fv1%2Fuser%2Fdefault-5&isVerified=false&teamName=natours">

# NATOURS_API
API to create , get , update and delete tours and also with users and reviews , backend api with all authentications , authorizations and security.
* start [API](https://documenter.getpostman.com/view/38505131/2sAXxWb9xb)

* Content of API
  * Tours (create , get , update , delete)
  * users (create , get , update , delete)
  * reviews (create , get , update , delete)
* these are for user resources
  * API support authentications , authorizations and security and you can
  * change password with 2 routes (changePassword , forgotPassword)
  * get user data (information account)
* these are for user resources
  * get monthly plan
  * get tour within specifis distance
  * make fields , limit , pagination , etc.....
  * use any logical oerations but look at documentation to understand how to use API
* these are for reviews resources
  * get review on specific tour
  * make review on specific tour
  * all staff for reviews
<hr>

![GET](https://img.shields.io/badge/GET-blue) getTour
### `/api/v1/tours/5c88fa8cf4afda39709c295d`
```
{
    "startLocation" : {
        "type" : "Point",
        "coordinates" : [15,15],
        "address" : "EGYPT",
        "description" : "hello from EGYPT"
    },
    "name" : "test test test test test test",
    "duration" : 5,
    "ratingsAverage" : 5,
    "maxGroupSize" : 15,
    "difficulty" : "easy",
    "price" : 500,
    "locations" : [
        {
            "coordinates" : [5,5]
        }
    ],
    "imageCover" : "png.png",
    "summary" : "test",
    "guides" : [
        "6706ed7c82d7532034c08d82",
        "6706ed8682d7532034c08d84"
    ]
}
```
![GET](https://img.shields.io/badge/GET-blue) createTour
### `127.0.0.1:3000/api/v1/tours`
```
 {
    "startLocation" : {
        "type" : "Point",
        "coordinates" : [15,15],
        "address" : "EGYPT",
        "description" : "hello from EGYPT"
    },
    "name" : "test test test test test test",
    "duration" : 5,
    "ratingsAverage" : 5,
    "maxGroupSize" : 15,
    "difficulty" : "easy",
    "price" : 500,
    "locations" : [
        {
            "coordinates" : [5,5]
        }
    ],
    "imageCover" : "png.png",
    "summary" : "test",
    "guides" : [
        "6706ed7c82d7532034c08d82",
        "6706ed8682d7532034c08d84"
    ]
}
```
<hr>

![POST](https://img.shields.io/badge/GET-blue) signup
### `127.0.0.1:3000/api/v1/users/signup`
```
 {
    "name" : "kareem9",
    "email" : "hello@kareem99999.io",
    "password" : "test1234",
    "passwordConfirm" : "test1234",
    "role" : "user"
}
```
![POST](https://img.shields.io/badge/GET-blue) login
### `127.0.0.1:3000/api/v1/users/login`
```
{
    "email" : "admin@natours.io",
    "password" : ".........."
}
```
![POST](https://img.shields.io/badge/GET-blue) forgotPassword
### `Natour.ioapi/v1/users/forgotPassword`
```
 {
    "email" : "hello@kareem.io"
}
```
![POST](https://img.shields.io/badge/GET-blue) resetPassword
### `Natour.ioapi/v1/users/resetPassword/f95e343329a31f3b81af15d455fc07929c7dc1d57be4175ff56a1f1e4339ac30`
```
 {
    "password" : "123456kareem",
    "passwordConfirm" : "123456kareem"
}
```
![POST](https://img.shields.io/badge/GET-blue) createReview
### `/api/v1/reviews`
```
 {
    "review" : "amazing!",
    "rating" : 5,
    "tour" : "6706f083d1888357882ab93d",
    "user" : "6706ed8682d7532034c08d84"
}
```

![POST](https://img.shields.io/badge/GET-blue) create review on tour
### `Natour.ioapi/v1/tours/5c88fa8cf4afda39709c295d/reviews`
```
 {
    "rating" : 4,
    "review" : "amazing tour !"
}
```
<br>
<hr>
 <h5>there are many routes and if you want to know them read documentation</h5>

 * start [API](https://documenter.getpostman.com/view/38505131/2sAXxWb9xb)
