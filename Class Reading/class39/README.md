# Class 39

## Reading  Questions

### 1. What is React Context, and how does it help in managing state and data sharing in a React application?

* React Context is a feature in React that provides a way to share state and data across components without the need to pass props manually through each level of the component tree. It allows you to create a global state that can be accessed by any component within a designated context, regardless of their position in the component hierarchy. Context is particularly useful when dealing with data that needs to be accessed by multiple components or when avoiding prop drilling becomes challenging.

### 2. Explain the useContext Hook and how it can be used to access data from a React Context within a functional component

The useContext hook is a React hook that allows functional components to consume data from a context created using the React.createContext function. It eliminates the need to wrap a component with the context consumer and provides a more concise way to access context data.

### Example of using useContext

```jsx
import React, { useContext } from 'react';
import { UserContext } from './UserContext';

function Profile() {
    const user = useContext(UserContext);
    
    return (
        <div>
            <h2>Welcome, {user.name}!</h2>
            <p>Email: {user.email}</p>
        </div>
    );
}
```

### 3. Describe the purpose of Next.js, and provide an example from the Vercel Next.js Examples reading on how it can be used to build a scalable web application

***Next.js:***

Next.js is a React framework designed to simplify and enhance the development of server-rendered React applications. It provides features like server-side rendering (SSR), static site generation (SSG), routing, and more, out of the box. Next.js improves performance by optimizing page loading and SEO through its built-in features. It allows developers to build scalable web applications with a focus on performance and user experience.

### Example

***CSS Styling and CSS Modules***

In the context of Next.js, CSS styling can be achieved through various methods, including CSS Modules. CSS Modules allow locally scoped CSS at the component-level, automatically generating unique class names to prevent class name collisions. This approach enhances code organization and reusability, making it easier to manage styles for individual components. Next.js supports other styling options as well, such as Sass, PostCSS libraries like Tailwind CSS, and CSS-in-JS libraries like styled-components.
