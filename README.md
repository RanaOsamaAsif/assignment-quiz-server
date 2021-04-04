# MCQ Quiz Server Assignment

In this assignment you have to create a simple MCQ Quiz application using React. 

In short your application is supposed to do the following

- Fetch the MCQ questions and their options from the API
- Allow the user to take the quiz
- Update the marks of user if he/she selects the correct option 

## Start the Server & Check the API
- Clone this repository and install the dependencies using `npm install`
- Run the API locally using the command `npm run api` This will start the demo server and the API endpoints will be available
- You can see the API `http://localhost:3333`
- Endpoint for questions `http://localhost:3333/question_list`
- Endpoint for options `http://localhost:3333/options_list`

## Details of React App
- Create a new react application
- Create a simple UI for showing questions to user and their choices. An example UI can be seen [Here](https://drive.google.com/file/d/19Cpg978r-i5JxCnyAOZvLJEJ897AZDpe/view?usp=sharing)
- Fetch the questions from `http://localhost:3333/question_list`
- Fetch the choices from `http://localhost:3333/options_list`
- Show user the marks, in the beginning they'll be zero
- When the user selects a correct option increase the marks 
- When the user selects a incorrect option deduct the marks

## Database Stucture
Careful understanding of database structure is important.

Questions have the following structure:

> {
      "id": 17, -> ID of question
      "points": 10, -> Marks of question
      "title": "Who is the Founder of Pakistan?" -> Title of Question
  }

Options have the following structure:

> {
      "id": 57, -> ID of option
      "title": "23 March", -> Name of option
      "related_question": 18, -> To which question this option belongs to
      "correct_answer_to_question": 18 -> This is the correct answer to the question whose ID is 18
  }

Note: If the `correct_answer_to_question` field is null that means that the option is incorrect and no marks will be given to the user.

## Submission
To submit your work you have to create a new Github repository and commit all your code. When your done share the url of the Github repo via email. 




