# React-Lab-Exercise-12-A-Simulating-a-Simple-SPA-Using-React

# Name : Moulishwar G
# Register Number : 2305001020

# Aim:
To create a simple Single Page Application (SPA) using React in which users can navigate between Home, About, Contact, Courses, and Student pages without reloading the entire webpage.

# Program:
## Home.jsx
```python
function Home() {
  return (
    <div>
      <h2>Home Page</h2>
      <p>Welcome to our React SPA!</p>
    </div>
  );
}

export default Home;

```

## about.jsx
```python
function About() {
  return (
    <div>
      <h2>About Page</h2>
      <p>This is a simple Single Page Application.</p>
    </div>
  );
}

export default About;

```
## Contact.jsx
```python
function Contact() {
  return (
    <div>
      <h2>Contact Page</h2>
      <p>Email: student@example.com</p>
    </div>
  );
}

export default Contact;

```
## App.jsx
```python
import { useState } from "react";
import Home from "./Home";
import About from "./About";
import Contact from "./Contact";
import Courses from "./Courses";
import Student from "./Student";
import "./index.css";

function App() {
  const [page, setPage] = useState("home");

  return (
    <div className="app">
      <h1>Simple React SPA</h1>

      <nav>
        <button onClick={() => setPage("home")}>Home</button>
        <button onClick={() => setPage("about")}>About</button>
        <button onClick={() => setPage("contact")}>Contact</button>
        <button onClick={() => setPage("courses")}>Courses</button>
        <button onClick={() => setPage("student")}>Student</button>
      </nav>

      <hr />

      {page === "home" && <Home />}
      {page === "about" && <About />}
      {page === "contact" && <Contact />}
      {page === "courses" && <Courses />}
      {page === "student" && <Student />}
    </div>
  );
}

export default App;
```

# Output:

<img width="1125" height="399" alt="702939490-68787147-a720-481c-8753-9453f4357d27" src="https://github.com/user-attachments/assets/2f389b48-ea66-4d3b-ae45-e2d36e70ce60" />

<img width="1125" height="378" alt="702939580-f09a82eb-0c43-4708-bb33-088a82ffbba6" src="https://github.com/user-attachments/assets/6c983ad1-16cc-49f7-82d4-8bc8cec1848f" />

<img width="1125" height="396" alt="702939691-da8af465-0583-4ddc-ae1f-587721b3dfec" src="https://github.com/user-attachments/assets/815e6d50-2a78-4b43-a2ac-c944b99211f3" />

# Result:
Thus, a simple Single Page Application was created successfully using React. The application allows users to navigate between Home, About, Contact, Courses, and Student pages dynamically without reloading the entire webpage.




