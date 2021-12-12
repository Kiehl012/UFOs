# Overview
The purpose of this project was to create an interactive webpage for UFO-enthusiasts to filter through UFO sightings. Users can input parameters like the date, city, state, etc and quickly see all sightings that match the given criteria.

# Result
The webpage includes an interactive javascript table. Users input parameters and as soon as they hit 'enter' or click away from the text box they were typing in, the table updates based on those parameters. The screenshot below shows the results after entering "1/12/2010" in the date field. </br>

![Screen Shot 2021-12-11 at 9 20 27 PM](https://user-images.githubusercontent.com/90878911/145698913-0f11d61a-cac6-4f15-a203-e34e6c2783ac.png) </br></br>

The next screenshot shows the results after adding a "state" parameter. With each additional parameter, users can further refine their search.</br>

![Screen Shot 2021-12-11 at 9 50 48 PM](https://user-images.githubusercontent.com/90878911/145699531-fbf4b3f8-883d-4b2a-a3f1-bfb1e5aff8c3.png)</br></br>

# Future Improvements

Though effective and simple, this webpage has a few drawbacks that could be improved upon. The first and most glaring is the sensitivity of the search terms. In the original specs for this project, there were no requirements for handling the inputs, meaning the program looked for exact matches, which can feel clunky and frustrating to users. The case-sensitivity is paricularly bothersome because state abbreviations are traditionally capitalized, yet in the table they are all lowercase. So, if a user enters "CA" for California instead of "ca", the program will return 0 results, which is not accurate. I actually ran into this issue myself while testing it, so I made sure that the program turns all user inputs to lower case before filtering the table. This is all done behind the scenes, so the user experience is unaffected.

With case-sensitivity solved for, the filters feel much more fluid, but there's still plenty of room to improve the user experience. Functionality could be added to accept inputs in multiple formats. For example, it'd be great if the "state" filter accepted states that are fully spelled out OR abbreviated rather than ONLY abbreviated. This saves the user from having to look up an abbreviation if they don't know it. Lastly, in it's current iteration, each filter only accepts one argument at a time, so if a user wanted to see sightings from multiple states, or from a range of dates, they would only be able to do so one-by-one, which isn't convenient. Additional functionality that can handle more than one value for each filter would make this a much more powerful tool.
