1/28/16 Morning Notes for Thistory

 user table
 -email
 -password
 -username

 user model
 -has_many :places, through: connectedplaces (Follow a place, Alerts?)
 -has_many :stories

 Admin table
 -email, password, username
 (if admin has same email as user there could be a toggle to switch between User and Admin mode.)

profile table
 -first_lastname(human)
 -Area of expertise(image upload, or dropdown menu)
 -bio
 -age range(state machine)

Location (neighborhood?)
has_many places

Places model
has_many :stories
belongs_to :location
(places are specific locations within neighborhoods.)
(Do places have different names? Used to be called something else.)
 How do we break down places?
 -States?, Cities?, Neighborhoods? GPS location? call a place whatever google calls a place?

Stories Model
-time period
-title
-sotry_text
-user_id
-place_id
-status(is it by a historian or is it by a grandma who used to live in that house?)

*validations*
50-200 chars(title)
belongs_to :place

Reference model
-boolean(is it factual or anecdotal.)

Verification of story with source or picture?
 -what about anecdotle stories?
 -do those posts look different?

 Something in between a user and an admin?
 -after a certain amount of posts they become a "super User". They are credible.

Who is allowed to search for a place on googlemaps and save it?
find a place. search for place by address or location. use that information lat/long or street adress and add a name or use the name that google provides from googlemaps.
user goes on site searches an address not in our database. they can add that place with a title.

Stories somehow connected to other stories
auto populate certain areas information
walking tours
books?
ancestry.com(grandma's old house.)

Do we use Devise?

History channel already made the app.
Conflict drives traffic. 
Validating stories should be relaxed? Funny stories should be allowed?

 

In Greg we trust.











