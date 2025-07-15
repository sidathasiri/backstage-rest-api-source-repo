# Frequently Asked Questions (FAQ)

---

### Q: I cannot install packages correctly on my local machine. What should I do?

**A:** To install private packages, you must log in to AWS CodeArtifact. Please ensure your AWS credentials are configured locally. Then, run the following command to authenticate:

```sh
aws codeartifact login --tool npm --repository common-ts-libs --domain raintree-libs
```

After logging in, you can install packages as usual with:

```sh
npm install
```

If you continue to experience issues, double-check your AWS credentials and network connectivity.