# Authentication

You need to authenticate by logging into your Kloudlite account. This process ensures you have secure access to your projects and environments.

### Logging In

Open your terminal or command prompt to begin. To log in, execute the following command:

```sh
shCopy codekl auth login
```

After you run this command, you'll be prompted to enter your Kloudlite account credentials. Simply follow the instructions that appear on your screen to successfully log in.

### Logging Out

Should you need to log out from your Kloudlite account for any reason, you can easily do so with this command:

```sh
shCopy codekl auth logout
```

This ensures that your session is securely closed, preventing unauthorized access to your account details.

### Checking Status

To check if you are currently logged in and to see the status of your authentication, you can use:

```sh
shCopy codekl status
```

This command will display a summary of your current authentication status, including details about your account, the project you're working on, the environment you're connected to, and your current device.

#### Example Output

Running the `kl status` command will produce an output similar to this:

```less
lessCopy codeLogged in as Karthik Thirumalasetti (karthik@kloudlite.io)

Account: demo-341290
Project: samplep
Environment: sample
Device: karthiks-macbook-pro-817927 (Connected)
```

This indicates that you're successfully logged in to `kl`, and it provides specific details about your account, your active project, the environment you're working in, and the device you're currently using.
