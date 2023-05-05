# Assignment_Persist-Ventures

The code adds the Bootstrap stylesheet and uses the Bootstrap classes to style the form elements. The form now has a container element that centers it on the page and adds some padding. The form elements are wrapped in form-group divs, which provide some additional styling and spacing.

The buttons have also been styled with the Bootstrap classes btn and btn-primary for the "Prefill" button, and btn and btn-success for the "Submit" button. These classes give the buttons a more modern look and feel.

This code assumes that you have already created a MySQL database with a table called "users" that has columns for "name", "email", and "phone". You will need to replace the $servername, $username, $password, $dbname variables with your own database credentials.

The code starts by creating a database connection using the mysqli_connect() function. It then checks if the form has been submitted (i.e., the HTTP method is "POST"), and retrieves the form data from the $_POST superglobal variable.

The code then constructs an SQL query to insert the form data into the "users" table using the mysqli_query() function. If the query is successful, the code redirects the user to a "thank you" page using the header() function. If an error occurs, the code outputs the error message using the mysqli_error() function.

Finally, the code closes the database connection using the mysqli_close() function.
