Live Link:-https://notekeeper-application.netlify.app
About:- The Notes-Keeper web application is a React-based application designed to provide users with a convenient and intuitive way to manage their notes. It offers essential functionalities such as creating, reading, updating, and deleting notes.

From an interview perspective, it demonstrates the following key aspects:

1. React: The application is built using React, a popular JavaScript library for building user interfaces. This showcases your proficiency in React development and understanding of its core concepts such as components, state management, and rendering.

2. CRUD Operations: The app allows users to perform CRUD (Create, Read, Update, Delete) operations on notes. This showcases your ability to implement essential data manipulation functionalities using React and other related technologies such as JavaScript, HTML, and CSS.

3. User Experience: The application focuses on providing a user-friendly experience by offering a straightforward and intuitive interface for managing notes. It demonstrates your understanding of user-centric design principles and your ability to create an intuitive UI/UX.

4. Voice Integration: One unique feature of the application is the ability to add notes using voice input. This highlights your capability to integrate external technologies or APIs, such as speech recognition, into your application. It shows your adaptability and willingness to explore new technologies and enhance user experiences.

5. Code Organization and Best Practices: The application's codebase should showcase good organization, structure, and adherence to best practices. This includes using modular components, following coding conventions, and implementing proper error handling. It demonstrates your proficiency in writing clean and maintainable code.

6. Testing: Ideally, the application should include a testing strategy that covers different aspects, such as unit testing for individual components and integration testing for overall functionality. This showcases your understanding of testing methodologies and your commitment to delivering quality software.

Overall, the Notes-Keeper web application serves as an excellent demonstration of your skills in React development, data management, user experience design, integration of external technologies, code organization, and testing. It reflects your ability to build practical and user-friendly applications while following industry best practices.



Additionally, the project includes a voice notes feature. It uses the Web Speech API to enable voice recognition. The application listens for voice input and transcribes it into text. The transcribed text is displayed in a "Current Note" section. Users can save the transcribed note by clicking the "Save Note" button. The saved notes are displayed in a separate section.

The voice notes feature allows users to dictate notes using their voice instead of typing them manually. Here's how it works:

The code initializes the SpeechRecognition object by checking if the browser supports the Web Speech API and creating an instance of the SpeechRecognition object accordingly.

The SpeechRecognition object is configured with certain properties:

continuous is set to true, which means the recognition continues listening for speech until explicitly stopped.
interimResults is set to true, which allows capturing intermediate results as the user speaks.
lang is set to 'en-US' to specify the language for speech recognition (in this case, English).
The state variables isListening and note are initialized using the useState hook. isListening represents whether the microphone is actively listening for speech, and note stores the transcribed text.

The useEffect hook is used to start and stop the speech recognition based on the isListening state. When isListening is true, the microphone starts listening for speech, and when it's false, the microphone stops.

Inside the useEffect hook, event listeners are set up to handle various events of the SpeechRecognition object:

onstart event is triggered when the speech recognition starts, and a corresponding console log is printed.
onresult event is triggered when the speech recognition receives a result. The event contains an array of results, and the transcribed text is extracted from the results and stored in the note state variable.
onerror event is triggered if there is an error during the speech recognition process, and the error is logged to the console.
Two helper functions are defined: handleListen and handleSaveNote.

handleListen starts or stops the speech recognition based on the isListening state. If isListening is true, the microphone starts listening, and if it's false, the microphone stops.
handleSaveNote is called when the user wants to save the transcribed note. It adds the note to the savedNotes array and clears the note state.
In the JSX code, a section with class "box" is added to the existing layout. It displays the current note being transcribed. If isListening is true, a microphone emoji is shown; otherwise, a stop sign emoji is displayed. Buttons are provided to start/stop listening and to save the note. The transcribed note is displayed within a paragraph tag.

Another section displays the saved notes from the savedNotes array, with each note displayed in a separate paragraph tag.

Overall, the voice notes feature allows users to speak their notes, and the application transcribes the spoken words into text. Users can save the transcribed notes and view them alongside previously saved notes






# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
