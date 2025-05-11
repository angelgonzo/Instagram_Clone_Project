# Instagram_Clone_Project

Hello, this is my Instagram (IG) Clone project in which I put to use my skills of SQL to the test.
The data that you see there is fake and is just used for practice while I try to answer some potential real-world question.
For this particular project the main skill I used was JOINS as JOINS tend to be a bit difficult to get a grasp of I tried to incorporate them as much as I can, but this project tried to cover a good amount of functions that SQL is built off such as GROUP BY, ORDER BY, LIMIT, and HAVING!

The IG clone has 7 different tables all which reference each other one way or another, making this a MANY to MANY relationship, and as closely as I could get it to be similar to what Instagrams schema could look like (lol I'm sure it is so complicated but who knows? Definitely not me!)

Here's the breakdown:

The Instagram Clone has about 100 different users that are either bots or 'real' people. The bots are definied as any user that has liked every single photo, because, that is what the bots do on Instagram just at an extreme rate.
Each user has a unique id that auto increments with every new user, it is a primary key, and much like Instagram, my users all must have UNIQUE usernames to be refered by! Lastly, it contains a timestamp so we know when the users created their account

What would an Instagram Clone be without the photos we upload to them, probably just a forum board. The IG clone contains a photos table of about 257 individual photos that are referenced to the users who 'uploaded' them. Each of the photos have an ID, and an image url, along side a timestamp of their creation.

Given that every person has an opinion on something, why not let them express that opinion with comments! The IG clone has a comment table that contains the text, the timestamp, a unique id, and has the id's of the users and the photos they are attachted to. We can't have random comments popping up without a face to associate them with.
The comments table is the least utilized table for this project, but I stil wanted to include it out of the fact that Instagram has it. 

Likes! The IG clone has likes which are super important for our users to know when they posted an amazing photo. The likes table is special because it is mainly comprised of foreign keys, but as well as a primary key??? Yes, we use the primary key in this case to ensure that a single user can only like a photo once. Can you image if you could like your own photos more than once? Wild. In this table you will see that certain users have liked all the photos within our database, now it is possible that someone could potentially like every single photo on Instagram but there's an estimated 95 million pictures uploaded everyday, so by the time you're done with the first 95 million they'll be a billion new ones. Regardless, the bots in general are able to do this at an impressive speed, so we shall see a similar situation in this table as well.

What's a follower to a followee if not your biggest fan! The IG clone contains such fans mainly being composed out of FORGEIN KEYS referencing the users table, because how else could this function work? Like the likes table, this table also contains a PRIMARY KEY in which it prevents a an account from being followed by the same user with multple instances. Basically 1 follow button press per user!

What's the best tag to use for your photo so people can stumble upon it? I'm not sure, but what I am sure of is that my tags table is comprised of 21 tags, each with their own ID and name associated with it. I only chose 21 because that's all I could think of but as you know any word could be a tag, so technically we could have an infinite number of tags as long as we keep switching languages or making new words. Besides that though, this table is really simple as it will just store our tags. I figured this is a simple of version of how Instragram might have their own tags stored, but I could be wrong and they could have the database just liked to a bunch of dictionaries. 

Lastly, the photo_tags table is what I used to reference tags from the tags table to the tags found in the photos.

This pretty much is my entire project, and the rest are a few questions designed to showcase my skills, but like stated early to get a glimpse of what a company could be asking for, either to do a promotion, to send emails, or whatever companies do with your data.

Thank you for taking the time to look at this project!

