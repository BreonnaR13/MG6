# MG6

1. I think that if you write a for loop within an update method, the for loop will completely execute before running the update method again. I assume this because typically, a for loop will have to finish executiing all the way before the code moves onto the next command. I think maybe if the for loop takes a really long time, it may cause a lag because the update method takes longer to go through so any feature dependant on the update method may be a little delayed.

2. The way I implemented the feature to be able to pass through the underside of the platforms is by checking if the velocity of the cat using the rigidbody component. If the cat's velocity in the y direction was positive, menaing the cat is going upwards, I made it so that the collider of the cat gets disabled that way it can just pass through the playform when going up. One issue I noticed is that, if the platform is thick, then when the cat is coming back down even when it does not reach the top surface of the platform, the cat still makes it onto the platform. This would be because as the velocity becomes negative again, the collider is enabled once more making the cat not passble to the platform again.

