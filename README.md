# Package-Delivery-Algorithm

This project was assigned as part of my Data Structures & Algorithms II course.

The purpose of this project is to determine the best route and delivery distribution for the a parcel service. There are 40 packages that must be split up across two trucks with 3 different drivers. Some packages have delivery constraints, and some have been delayed. Additionally, there is a package that initially has the wrong address and packages that must go out on the second truck.

A series of conditional statements are used to load the trucks based on the data that is provided. A greedy algorithm is used to optimize delivery of each package along the truck route. This algorithm is greedy because it determines the shortest available path from its current location then continues to do this until no additional packages remain.

**Algorithm Overview:**

The greedy algorithm is executed by doing the following
1. A list of packages on the truck is passed in along with the associated truck number and the current location (always at hub by default)
2. The current location is compared to the locations of all the packages in the truck to determine the closest location.
3. The lowest value is determined once all objects in the truck have been compared then that value is removed from the truck list and the truck moves to that address location
4. That value is appended to an optimized location list than the algorithm updates current location with the new address and calls the function again with the smaller truck list.
