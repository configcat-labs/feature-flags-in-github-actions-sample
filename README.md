# feature-flags-in-github-actions-sample

This is the companion repository for the article Feature Flags in GitHub Actions: Run Jobs Dynamically.

Following the steps in the article, you can use a feature flag to run or skip the build and deploy jobs in this repository.

## Build & Run

**Prerequisite:** Working knowledge of GitHub and GitHub Actions

1. Fork this repository.
2. Log in to your [ConfigCat dashboard](https://app.configcat.com/), or sign up for the [Forever Free plan](https://configcat.com/pricing) if you don't have an account.
3. Create a feature flag with the following details:
    - **Name:** Build and deploy blog
    - **Key:** `build_deploy_enabled`
    - **Hint:** Allows the build and deploy jobs to run in my blog's GitHub Action workflow.
4. Click **SAVE & PUBLISH CHANGES**.

### Get your ConfigCat SDK key

1. Click **VIEW SDK KEY** in the top right corner of the dashboard.
2. Copy the SDK key and store it somewhere safe.

### Get your ConfigCat API credentials

1. Click the avatar icon in the top-left corner, then click **My API Credentials** in the dropdown that appears.   
2. Click **ADD CREDENTIAL**, give the credential a name, then click **CREATE**. A username and password will be generated.
3. Copy your credentials and store them somewhere safe.

### Add the SDK key and API credentials to your repository's environment secrets

1. Enter your forked repository's environment and select the `github-pages` environment. You can create the environment if it doesn't exist.
2. Add the following secrets to the environment:
    - `CONFIGCAT_SDK_KEY`: Your ConfigCat SDK key.
    - `CONFIGCAT_API_USER`: Your ConfigCat API username.
    - `CONFIGCAT_API_PASS`: Your ConfigCat API password.

### Run the workflow
Go to the **Actions** tab, select **Deploy static content to pages** from the left sidebar, and run the workflow manually.

## Learn more

- [ConfigCat GitHub Actions](https://github.com/configcat/cli-actions)
- [ConfigCat integrations](https://configcat.com/docs/integrations/overview/)

[**ConfigCat**](https://configcat.com) supports many other frameworks and languages. Check out the full list of supported SDKs [here](https://configcat.com/docs/sdk-reference/overview/).

You can also explore other code samples for various languages, frameworks, and topics in [ConfigCat labs](https://github.com/configcat-labs) on GitHub.

Keep up with ConfigCat on [X](https://x.com/configcat), [Facebook](https://www.facebook.com/configcat), [LinkedIn](https://www.linkedin.com/company/configcat/), and [GitHub](https://github.com/configcat).

## Author

[Zayyad Muhammad Sani](https://github.com/Z-MS)

## Contributions

Contributions are welcome!