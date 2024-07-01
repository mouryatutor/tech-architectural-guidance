# Full-stack dev setup of Spring Boot and React

1. <h3>Setup Your Environment: </h3>
    
    - Make sure you have Node.js, Java (at least version 8), and an IDE (such as IntelliJ IDEA for Spring Boot and Visual Studio Code for React) installed on your system.

2. <h3> Create a Spring Boot Project: </h3>

    - Go to Spring Initializer and create a new Spring Boot project.
    Add the “Web” dependency to your project.
    - Set the groupId and artifactId according to your preference.
    - Generate the project and unzip it into your project directory.

3. <h3> Create a React Frontend : </h3>

    - In your project directory, create a new folder for your React frontend.
    - Open a terminal and navigate to the frontend folder.
    - Run the following command to create a new React app:

            npx create-react-app my-app

    - Replace my-app with your desired app name.
    - Navigate into the newly created app folder: 
        
            cd my-app

4. <h3>Configure Proxy for Development</h3>

    - In your React app’s package.json, add the following line to set up a proxy to your Spring Boot backend (assuming it runs on port 8080):
        
            "proxy": "http://localhost:8080"
    
    - This allows your React app to communicate with the backend during development.

5. <h3>Build Your React App:</h3>

    - In the same terminal, run:

            npm start
6. Create Backend APIs with Spring Boot:

    - Create your Spring Boot controllers, services, and repositories to define your backend APIs.
    - Use annotations like @RestController and @RequestMapping to map endpoints
    - Implement your business logic and connect to your data source (e.g., a database).

7. Integrate React with Spring Boot:
    
    - In your React app, make API requests to your Spring Boot backend using libraries like Axios or Fetch.
    - For example, if you have an endpoint /api/posts in your Spring Boot app, you can fetch data from it in your React components.

8. Build and Package Your Application:

    - When you’re ready to deploy, build your React app:

            npm run build
    - This generates optimized production-ready files in the build folder.
    - Now, package your Spring Boot app and include the React build output:
        
        * You can use tools like Maven or Gradle to create a single JAR file containing both the backend and frontend.
        
        * Refer to resources like [this guide](https://dev.to/arpan_banerjee7/run-react-frontend-and-springboot-backend-on-the-same-port-and-package-them-as-a-single-artifact-14pa) for packaging them together






    


