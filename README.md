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

<h1>this is an examples on tour route to choose specific fields</h1>
<code>127.0.0.1:3000/api/v1/tours?fields=name,price,duration</code>
<code>127.0.0.1:3000/api/v1/tours/5c88fa8cf4afda39709c295d</code>
<code>127.0.0.1:3000/api/v1/tours/best-5-tours</code>
<code>127.0.0.1:3000/api/v1/tours/tours-within/distance/950/center/34.050653, -118.240979/unit/km</code>
<code>127.0.0.1:3000/api/v1/tours/distances/center/34.050653,-118.240979/unit/kg</code>
<br>
<h1>this is an examples on user route to choose specific fields</h1>
<code>127.0.0.1:3000/api/v1/users</code>
<code>127.0.0.1:3000/api/v1/users/6706ed8d82d7532034c08d86</code>
<code>127.0.0.1:3000/api/v1/users/signup</code>
<code>127.0.0.1:3000/api/v1/users/forgotPassword</code>
<code>127.0.0.1:3000/api/v1/users/resetPassword/f95e343329a31f3b81af15d455fc07929c7dc1d57be4175ff56a1f1e4339ac30</code>
<br>
<h1>this is an examples on review route to choose specific fields</h1>
<code>127.0.0.1:3000/api/v1/reviews</code>
<code>127.0.0.1:3000/api/v1/reviews?rating[gte]=5</code>
<code>127.0.0.1:3000/api/v1/tours/5c88fa8cf4afda39709c295d/reviews</code>
<code>127.0.0.1:3000/api/v1/reviews/6712c2dc2cd0d722e00e79d5</code>
<code>127.0.0.1:3000/api/v1/tours/6706f083d1888357882ab93d/reviews</code>
<br>
