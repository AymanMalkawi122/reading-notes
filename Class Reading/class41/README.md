# Class 41

## Reading  Questions

### 1. Explain the concept of dynamic routes in Next.js and how they differ from static routes?

* Static routes are defined by creating files in the pages directory, and each file corresponds to a specific route. They are suitable for pages that don't change frequently and don't require data fetching. Dynamic routes, on the other hand, allow for more flexibility as they generate pages dynamically based on parameters. This is particularly useful when dealing with data-driven content like blog posts, products, or user profiles. Dynamic routes also enhance code reusability by allowing a single page component to handle different data based on the parameter.

### 2. Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?

1.  Build the Application: Use the `next build` command to build the application, which generates optimized production-ready assets.

2.  Choose a Deployment Platform: Choose a hosting platform that supports Next.js applications. Platforms like Vercel, Netlify, and AWS Amplify are popular choices.

3.  Configure Deployment: Connect your repository to the chosen deployment platform. Configure build settings, environment variables, and other deployment-related options.

4.  Deploy: Trigger the deployment process on the platform. The platform will run the build process and deploy the application.

5.  Domain Setup: Configure your custom domain or use a provided subdomain for your deployed application.

Deployment Platforms: Some popular deployment platforms for Next.js applications include:

-   Vercel: Offers seamless integration with Next.js, providing automatic deployments and built-in features like serverless functions and preview deployments.
-   Netlify: Supports static site hosting with easy continuous deployment and custom domain setup.

### 3. How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application

Next.js provides a default folder called public for serving static assets. Files placed in the public folder are accessible by their filename in the root URL. For example, a file named logo.png in the public folder can be accessed at /logo.png. This approach is suitable for images, fonts, and other assets that don't require server-side processing. Including assets this way ensures efficient caching and optimized loading. When referencing static assets in Next.js, it's important to use the correct relative paths, considering the base URL of the application.
