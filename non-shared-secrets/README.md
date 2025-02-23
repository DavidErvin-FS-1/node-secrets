# Non-Shared Secrets

This method involves storing secrets in a separate configuration file that is not included in the version-controlled repository.

## Implications:

- Enhanced Security: Secrets are not stored in the codebase or repository, reducing the risk of exposure.

- Deployment Flexibility: Different environments (development, testing, production) can have distinct configurations without changing the code.

- Operational Overhead: Requires proper management of environment variables across different deployment platforms.

---

You will need to create an `.env` file in this directory with the following variables:

```bash
SECRET_KEY= 'enter_your_secret_key'
```

### Why Use a Dot (.) in Front of the .env File?

Files prefixed with a dot are hidden by default in Unix-based systems. Naming the environment file .env helps prevent accidental exposure and signifies that it contains configuration settings. Additionally, it's standard practice to add .env to your .gitignore file to exclude it from version control, ensuring that sensitive information doesn't get committed to the repository.
