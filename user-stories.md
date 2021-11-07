# User stories

Effort is specified in numbers from the fibonacci-range.

| 1    | 2    | 3    | 5    | 8    | 13   | 21   |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |

## Student

| ID   | User story (As a student I need)                                                                                                        | BV    | Effort       |
| :--- | :-------------------------------------------------------------------------------------------------------------------------------------- | :---- | :----------- |
| 1    | to be able to be logged in with my student-account using moodle-auth                                                                    | Must  | -            |
| 1.1  | Display login-view if the user is not authenticated                                                                                     | Must  | **1 (base)** |
| 1.2  | Handle login from external source (IOS-app) with the "User key authentication"-plugin                                                   | Must  | 5            |
| 2    | to be able to log myself out of the IOS-app                                                                                             | Must  | -            |
| 2.1  | Display logout-button inside the collapsible hamburger-menu                                                                             | Must  | 1            |
| 2.2  | Once the logout-button is clicked remove stored user-key from storage and memory                                                        | Must  | 2            |
| 2.3  | Display the login-view                                                                                                                  | Must  | 1            |
| 3    | to be able to access the 2D/3D-representation and sound of previous collected SOSs                                                      | Must  | -            |
| 3.1  | Display SOS-inventory button in the collapsible hamburger-menu                                                                          | Must  | 1            |
| 3.2  | Once the SOS-inventory is tapped display all previously collected SOSs (wave-form and 2D/3D visuals)                                    | Must  | 3            |
| 3.3  | Play the sound of SOS when play-icon is tapped                                                                                          | Must  | 1            |
| 3.4  | Show a larger representation of the 2D/3D visuals once tapped                                                                           | Must  | 1            |
| 4    | the mascot to help me at the beginning (Tutorial for first SOS)                                                                         | Must  | -            |
| 4.1  | Translation-middleware to translate german-text into german sign-writing (use API)                                                      | Must  | 2            |
| 4.2  | Show the mascot at the GUI-controls (around wave-form) while displaying the explanation from the translation-middleware                 | Must  | 2            |
| 4.3  | Display the mascot while the volume changes with translated explanation                                                                 | Must  | 2            |
| 4.4  | Display the mascot once the SOS is visible to explain to tap on the SOS                                                                 | Must  | 3            |
| 4.5  | Display the mascot during the captcha mini-game to explain it with sign writing                                                         | Must  | 3            |
| 4.6  | Display the mascot at the end of the tutorial (finished mini-game) to wish the player good luck with the next SOSs                      | Must  | 1            |
| 5    | to see and control the representation of the sound (wave-form)                                                                          | Must  | -            |
| 5.1  | Generate a visual wave-representation from the associated MP3-file (from scratch)                                                       | Must  | 8            |
| 5.2  | Build UI-elements around the wave-display to control the sound using icons (play, pause, repeat)                                        | Must  | 1            |
| 5.3  | Synchronise the sound-progress of the wave-representation and the IOS-sound component                                                   | Must  | 3            |
| 6    | the volume of the sound to adapt to the distance to the SOS                                                                             | Must  | -            |
| 6.1  | Request access to GPS-module from the user (only once)                                                                                  | Must  | 1            |
| 6.2  | Using the GPS-location of the device, calculate the distance (in meters) from the iPad to the SOS (without object-detection)            | Must  | 5            |
| 6.3  | Change the volume of the sound to be found according to the calculated distance (larger distance->lower volume & reverse)               | Must  | 2            |
| 7    | to be able to see and tap the SOS when I am close enough                                                                                | Must  | -            |
| 7.1  | The visual representation of the SOS is initially hidden                                                                                | Must  | 1            |
| 7.2  | Once the distance < 2m (its a range since GSP is not that accurate) show the visual representation of the SOS                           | Must  | 3            |
| 7.3  | Create 3D-representation of the room (using the camera and ARKit by iOS12)                                                              | Could | 5            |
| 7.4  | Display the SOS at the exact chosen position inside the world-matrix of the generated model of the room (that the teacher/parent chose) | Could | 8            |
| 8    | to play a captcha mini-game                                                                                                             | Must  | -            |
| 8.1  | Display the mini-game once the visual representation of the SOS has been tapped                                                         | Must  | 1            |
| 8.2  | Show visual representations of SOSs and play the sound of one of them                                                                   | Must  | 3            |
| 8.3  | If the player taps on the wrong visual representations of SOS 3 times, help the player with a hint.                                     | Must  | 2            |
| 9    | to be celebrated by the mascot once the mini-game is won                                                                                | Must  | -            |
| 9.1  | Create 10 different celebration-scenarios including the mascot and different sounds                                                     | Must  | 3            |
| 9.2  | Display a random celebration-scenario from the created set of 10                                                                        | Must  | 1            |
| 10   | the mascot to help me when I'm stuck                                                                                                    | Must  | -            |
| 10.1 | Display a button in the form of a help-icon inside the GUI                                                                              | Must  | 1            |
| 10.2 | Show the mascot with an explanation of the current step in the game (sign-writing)                                                      | Must  | 3            |
| 11   | to get a new sound assigned once I finish the previous one                                                                              | Must  | -            |
| 11.1 | Add collected SOS to players inventory                                                                                                  | Must  | 2            |
| 11.2 | Randomly pick new SOS to be used in the next iteration                                                                                  | Must  | 1            |
| 11.3 | Show new wave-form to the player                                                                                                        | Must  | 1            |
| 12   | my progress to persist (device- and account independent)                                                                                | Must  | -            |
| 12.1 | Use the user key to be able to access the game-routes of moodle                                                                         | Must  | 2            |
| 12.2 | Use moodle's REST-plugin to make http-based requests containing progress-data of the player                                             | Must  | 5            |

## Teacher/Parent

| ID   | User story (As a teacher/parent I need)                                                                     | BV    | Effort |
| :--- | :---------------------------------------------------------------------------------------------------------- | :---- | :----- |
| 1    | to be able to be logged in with my editor-account using moodle-auth                                         | Must  | -      |
| 1.1  | Display login-view if the user is not authenticated                                                         | Must  | 1      |
| 1.2  | Handle login from external source (IOS-app) with the "User key authentication"-plugin                       | Must  | 5      |
| 2    | to be able to edit the SOSs in the location in my responsibility (school/home)                              | Must  | -      |
| 2.1  | Request access to GPS-module from the user                                                                  | Must  | 1      |
| 2.2  | Create routes to support CRUD-operations for SOSs as resources (backend)                                    | Must  | 8      |
| 2.3  | Create button to set a new SOS at the current GPS-location                                                  | Must  | 1      |
| 2.5  | Once the button is tapped display a "create-new-SOS-form"                                                   | Must  | 1      |
| 2.6  | Create 3D-representation of the room (using the camera and ARKit by iOS12)                                  | Could | 5      |
| 2.7  | Let the user choose position inside the 3D-Model where the SOS should be placed                             | Could | 8      |
| 2.8  | Save the 3D-representation of the room together with the picked position for the SOS inside the form        | Could | 5      |
| 2.9  | Provide GUI-elements for attaching sound from own library                                                   | Must  | 2      |
| 2.10 | Provide GUI-elements for picking sound from shared-repository                                               | Must  | 3      |
| 2.11 | Provide GUI-elements for attaching 2D-image from own library                                                | Must  | 2      |
| 2.12 | Provide GUI-elements for attaching 2D-image from shared-repository                                          | Must  | 3      |
| 2.13 | Provide GUI-elements for attaching 3D-model from shared-repository                                          | Must  | 3      |
| 2.14 | Create button to submit new SOS (containing sound, visual representation & location)                        | Must  | 1      |
| 2.15 | Once tapped make authenticated request to the SOS-creation server-endpoint                                  | Must  | 2      |
| 3    | to monitor the progress of the kid/s in the browser                                                         | Must  | -      |
| 3.1  | Add new Menu-button to the hamburger menu                                                                   | Must  | 1      |
| 3.2  | Once that button is tapped display the kids in your responsibility                                          | Must  | 2      |
| 3.4  | When a kid is selected show 2D-stats of the progress (number of SOSs collected with time)                   | Must  | 3      |
| 4    | to monitor the progress of the kid/s in the IOS-app                                                         | Must  | -      |
| 4.1  | Add new Menu-button to the hamburger menu                                                                   | Must  | 1      |
| 4.2  | Once that button is tapped display the kids in your responsibility                                          | Must  | 2      |
| 4.4  | When a kid is selected show 2D-stats of the progress (number of SOSs collected with time)                   | Must  | 3      |
| 5    | a grievance-section to know about the feelings of the kids towards parts of the game                        | Could | -      |
| 5.1  | Add routes to submit and get ratings with the moodle REST-plugin                                            | Could | 2      |
| 5.2  | After collecting a SOS display a star-rating (1-5 since the kids cannot read)                               | Could | 1      |
| 5.3  | Once the player taps a star the rating is submitted to the according backend-route                          | Could | 2      |
| 5.4  | Add Button in the moodle-plugin (Inside the browser) to access the ratings by the students                  | Could | 1      |
| 5.5  | Once the button is clicked display the ratings from the players in the responsibility of the teacher/parent | Could | 2      |
