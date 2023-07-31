# Class 34

## Reading  Questions

### 1. What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading?

Use Multiple Settings Files: Split settings into multiple files, such as base settings, development settings, and production settings, to manage different configurations for different environments.

Environment-Specific Settings: Use environment variables to store sensitive and environment-specific settings, making it easier to switch between different configurations.

Keep Secrets Secure: Store sensitive information like API keys, database credentials, and secret keys in environment variables or use tools like python-decouple to store them externally.

Avoid Hardcoding: Avoid hardcoding values in settings and instead use environment variables or constants to make the code more maintainable.

### 2. How does the White Noise library contribute to the efficient serving of static files in a Django application, and what are the steps to integrate it into a project?

The White Noise library is a Python package that allows Django applications to efficiently serve static files directly from the web server. By serving static files through the web server rather than Django, it reduces the overhead on the Django application, leading to improved performance and efficiency.

```python
STATIC_URL = '/static/'
STATIC_ROOT = os.path.join(BASE_DIR, 'staticfiles')
STATICFILES_STORAGE = 'whitenoise.storage.CompressedManifestStaticFilesStorage'
```

### 3. What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources?

Cross-Origin Resource Sharing (CORS) is a security feature implemented by web browsers to control access to resources on different origins (i.e., different domains, protocols, or ports). It is designed to prevent unauthorized access to resources and protect against cross-site request forgery (CSRF) and other potential security risks.

With CORS configured, the Django application will send appropriate CORS headers in responses, allowing the web browser to control access to resources and prevent unauthorized cross-origin requests.
