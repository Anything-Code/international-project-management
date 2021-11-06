# User stories

Effort is specified in numbers from the fibonacci-range.

| 1    | 2    | 3    | 5    | 8    | 13   | 21   |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |

## Student

| ID   | User story (As a student I need)                                                                                    | BV   | Effort |
| :--- | :------------------------------------------------------------------------------------------------------------------ | :--- | :----- |
| 1    | to be able to be logged in with my student-account using moodle-auth                                                | Must |        |
| 1.1  | Display login-view if the user is not authenticated                                                                 | Must |        |
| 1.2  | Handle login from external source (IOS-app) with the "User key authentication"-plugin                               | Must |        |
| 2    | to be able to log myself out of the IOS-app                                                                         | Must |        |
| 2.1  | Display logout-button inside the collapsible hamburger-menu                                                         | Must |        |
| 2.2  | Once the logout-button is clicked remove stored user-key from storage and memory                                    | Must |        |
| 2.3  | Display the login-view                                                                                              | Must |        |
| 3    | to be able to access the 2D/3D-representation and sound of previous collected SOSs                                  | Must |        |
| 3.1  | Display SOS-inventory button in the collapsible hamburger-menu                                                      | Must |        |
| 3.2  | Once the SOS-inventory is tapped display all previously collected SOSs (wave-form and 2D/3D visuals)                | Must |        |
| 3.3  | Play the sound of SOS when play-icon is tapped                                                                      | Must |        |
| 3.4  | Show a larger representation of the 2D/3D visuals once tapped                                                       | Must |        |
| 4    | the mascot to help me at the beginning (Tutorial for first SOS)                                                     | Must |        |
| 4.1  | Translation-middleware to translate german-text into german sign-writing                                            | Must |        |
| 4.2  | Move the mascot to the GUI-controls (wave-form) while displaying the explanation from the translation-middleware    | Must |        |
| 4.3  | Display the mascot while the volume changes with translated explanation                                             | Must |        |
| 4.4  | Display the mascot once the SOS is visible to explain to tap on the SOS                                             | Must |        |
| 4.5  | Display the mascot during the captcha mini-game to explain it with sign writing                                     | Must |        |
| 4.6  | Display the mascot at the end of the tutorial (finished mini-game) to wish the player good luck with the next SOSs  | Must |        |
| 5    | to see and control the representation of the sound (wave-form)                                                      | Must |        |
| 5.1  | Generate a visual wave-representation from the associated MP3-file                                                  | Must |        |
| 5.2  | Build UI-elements around the wave-display to control the sound using icons (play, pause, repeat)                    | Must |        |
| 6    | the volume of the sound to adapt to the distance to the SOS                                                         | Must |        |
| 6.1  | Request access to GPS-module from the user                                                                          | Must |        |
| 6.2  | Using the GPS-location of the device, calculate the distance (in meters) from the iPad to the SOS                   | Must |        |
| 6.3  | Change the volume of the sound to be found according to the calculated distance (larger distance->lower volume & !) | Must |        |
| 7    | to be able to see and tap the SOS when I am close enough                                                            | Must |        |
| 7.1  | The visual representation of the SOS is initially hidden                                                            | Must |        |
| 7.2  | Once the distance < 2m show the visual representation of the SOS                                                    | Must |        |
| 8    | to play a captcha mini-game                                                                                         | Must |        |
| 8.1  | Display the mini-game once the visual representation of the SOS has been tapped                                     | Must |        |
| 8.2  | Show 9 visual representations of SOSs and play the sound of one of them                                             | Must |        |
| 8.4  | If the player taps on the wrong visual representations of SOS 3 times...                                            | Must |        |
| 9    | to be celebrated by the mascot once the mini-game is won                                                            | Must |        |
| 9.1  | Create 10 different celebration-scenarios including the mascot and different sounds                                 | Must |        |
| 9.2  | Display a random celebration-scenario from the created set of 10                                                    | Must |        |
| 10   | the mascot to help me when I'm stuck                                                                                | Must |        |
| 10.1 | Display a button in the form of a help-icon inside the GUI                                                          | Must |        |
| 10.3 | Show the mascot with an explanation of the current step in the game (sign-writing)                                  | Must |        |
| 11   | to get a new sound assigned once I finish the previous one                                                          | Must |        |
| 11.1 | Add collected SOS to players inventory                                                                              | Must |        |
| 11.2 | Pick new SOS to be used in the next iteration                                                                       | Must |        |
| 11.3 | Show new wave-form to the player                                                                                    | Must |        |
| 12   | my progress to persist (device- and account independent)                                                            | Must |        |
| 12.1 | Use the user key to be able to access the game-routes of moodle                                                     | Must |        |
| 12.2 | Use moodle's REST-plugin to make http-based requests containing progress-data of the player                         | Must |        |

## Teacher/Parent

| ID   | User story (As a teacher/parent I need)                                                   | BV   | Effort |
| :--- | :---------------------------------------------------------------------------------------- | :--- | :----- |
| 1    | to be able to be logged in with my editor-account using moodle-auth                       | Must |        |
| 1.1  | Display login-view if the user is not authenticated                                       | Must |        |
| 1.2  | Handle login from external source (IOS-app) with the "User key authentication"-plugin     | Must |        |
| 2    | to be able to edit the SOSs in the location in my responsibility (school/home)            | Must |        |
| 2.1  | Request access to GPS-module from the user                                                | Must |        |
| 2.2  | Create routes to support CRUD-operations for SOSs as resources                            | Must |        |
| 2.3  | Create button to set a new SOS at the current GPS-location                                | Must |        |
| 2.5  | Once the button is tapped display a "create-new-SOS-form"                                 | Must |        |
| 2.6  | Provide GUI-elements for attaching sound from own library                                 | Must |        |
| 2.7  | Provide GUI-elements for picking sound from shared-repository                             | Must |        |
| 2.8  | Provide GUI-elements for attaching 2D-image from own library                              | Must |        |
| 2.9  | Provide GUI-elements for attaching 2D-image from shared-repository                        | Must |        |
| 2.10 | Provide GUI-elements for attaching 3D-model from shared-repository                        | Must |        |
| 2.11 | Create button to submit new SOS (containing sound, visual representation & location)      | Must |        |
| 2.13 | Once tapped Make authenticated request to the SOS-creation server-endpoint                | Must |        |
| 3    | to monitor the progress of the kid/s in the browser                                       | Must |        |
| 3.1  | Add new Menu-button to the hamburger menu                                                 | Must |        |
| 3.2  | Once that button is tapped display the kids in your responsibility                        | Must |        |
| 3.4  | When a kid is selected show 2D-stats of the progress (number of SOSs collected with time) | Must |        |
| 4    | to monitor the progress of the kid/s in the IOS-app                                       | Must |        |
| 4.1  | Add new Menu-button to the hamburger menu                                                 | Must |        |
| 4.2  | Once that button is tapped display the kids in your responsibility                        | Must |        |
| 4.4  | When a kid is selected show 2D-stats of the progress (number of SOSs collected with time) | Must |        |
