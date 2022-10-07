# Project ID: d1b8e34d-35d0-40fe-bc76-8451f9c01547

Write your documentation for the project below.

## Documentation

The name of the application is "Quiz time".

The application consists of three pages which are home page, question page and result page.
Home page contains clickable buttons for question topics retrieved from the API endpoint and 
Statistics section which shows the number of questions answered and the number of correct 
answers. By clicking a button, the user is navigated to the question page.

The question page shows the question and the answer options retrieved from the API endpoint. 
The answer options are clickable and by clicking some of them, the user is navigated to the 
result page. Some questions are about images and in that case an image is also shown in the 
question page. The user has also a possibility to return to the home page by clicking the 
"Back to topics" button.

The result page contains information about the correctness of the option. This information is 
once again retrieved from the API endpoint. In addition to that, the page contains the 
same Statistics section which is shown on the home page, "Back to topics" button for returning 
to home and "Show new question" button which moves the user to the question page of the 
currently selected topic. 

The application uses Riverpod to store the number of questions and correct answers. Package 
named go_router is used for routing. Desktop and mobile layouts are also implemented so that 
the desktop layout has larger buttons and font sizes. The statistics section is located on 
the right side of the screen when desktop layout is used and on the bottom of the screen when 
the mobile layout is used. The breakpoint between these two layouts is at 600px.

The application uses flutter widgets like Cards, ListTiles, ListViews, and GridViews to show 
content to the user. Also padding and margin are added for the elements when needed. When the 
screen width is larger than 1500px the layout is centered. The application is also deployed 
online and the online address of the application is https://toukolonka.github.io/quiz-time.

3 key challenges
1. Updating the provider state based on HTTP response
2. Reading Riverpod documentation which is not really good
3. Adjusting the size of elements and text based on screen size

3 key learning moments
1. Provider state cannot be updated inside the builder function of FutureBuilder
2. Using images and icons in your Flutter application is very simple
3. Centering the layout on wide screens makes the application feel more usable