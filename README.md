# Go Swag Front End Technical Assessment

Before starting the assessment ensure you have created an Angular project and loaded in a CSS library you are familiar
with.

The assessment should last around an hour, don't include Angular set up time in this, you should spend around 30 minutes
on each task, design and implementation.

## Design

For the design task you will require a free Figma account.

You are to implement one of the components either `Sidebar navigation`, `Main` or `Side panel`.

View the design at this link: https://www.figma.com/file/Cdy8JweRbP8kKFzhvIUUKL/Front-end-Task?type=design&mode=design

## Implementation

For this section do not worry about CSS / Design elements focus on the technical implementation details.

### Profile Page

You are required to build a profile page using Angular that integrates with three different HTTP endpoints.

#### Requirements

Create a profile page with the following components and features. Each endpoint should have a corresponding loading
spinner to indicate when data is being fetched.There is an example wire frame in the `images` directory.

Profile Information:

- Todos: Display and list the users todos from https://jsonplaceholder.typicode.com/users/1/todos
- Posts: Display a list of user posts from https://jsonplaceholder.typicode.com/users/1/posts
- Albums: Display a list of user albums obtained from https://jsonplaceholder.typicode.com/users/1/albums

If the endpoint is unavailable there is example data in the `mock_data` directory.

### Login Page

You will be responsible for building a simple login form that collects a username and password from the user and sends
this data to a server. The primary focus of this assessment is on your ability to work with Angular's form modules.

#### Requirements

Form Creation: Create an Angular component that includes a form with the following fields:

Username: A text input field.

Password: A password input field.

- Implement form validation to ensure that both the username and password fields are required. Display
  appropriate validation messages if the fields are empty.
- Implement form validation to ensure the password contains 1 upper case character.

HTTP Request: On form submission, you don't need to make an actual POST request simply `console.log` the payload, the
focus for this section is on reactive forms.

Success Message: Display a success message to the user once the server responds with a successful status (e.g., status
code 200).

Error Handling: Display an error message to the user if the server response indicates an error (e.g., status code 4xx or
5xx).

Clear Form: Clear the form fields after a successful submission.