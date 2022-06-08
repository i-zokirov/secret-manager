# secret-manager

SecretManager class with a couple of methods I use to create a secret value in [Secretmanager](https://cloud.google.com/secret-manager) and retrieve the value of stored secret for reuse.


## Documentation

In order to use the class methods, add GCP service account credentials to ./keys/secret-manager-key.json file. The service account must have Secret Manager Admin IAM role assigned in GCP project.

Two main methods you will ever need to use are **getSecret()** and **writeSecret()**. Their job is retrieve active value of the given secret and destroy previous values of secret when writing the value. **writeSecret()** creates a secret record with a given name if one was not previously created.

## License

[MIT](https://choosealicense.com/licenses/mit/)

Feel free to reuse, modify, distribute the code. Just don`t forget to leave ⭐️⭐️⭐️