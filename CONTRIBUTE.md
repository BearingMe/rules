# Guide for beginners contributors

## How to contribute?

To make contributions, make sure you have [git](https://git-scm.com/) installed in your environment. Then, follow those steps below.

### Fork

**Fork** the repository to your account by clicking on the fork button. It is located in the header inside any repository, just below its link.

### Clone

Once you've forked the project, you may be able to access it by using your own github account. After doing this, you should clone the repository on your machine.

```bash
$git clone https://github.com/<YOUR_ACCOUNT_NAME>/<REPOSITORY_NAME>.git
```

### Optional: Link fork to the official repository

This will be used to sync updates made in the official repository to your local environment. You might also update your forked repository manually on GitHub and then fetch it through git, making this step optional.

```bash
$git remote add upstream https://github.com/BlockLabz/<REPOSITORY_NAME>.git
```

This will serve to sync updates made in the official repository to your local environment.

> OBS: This command is only necessary to run once after cloning.

To check if everything went right, run the command below in the terminal:

```bash
$git remote --v
```

If everything went well, there should be an output similar to this:

```bash
origin  https://github.com/<YOUR_ACCOUNT_NAME>/<REPOSITORY_NAME>.git (fetch)
origin  https://github.com/<YOUR_ACCOUNT_NAME>/<REPOSITORY_NAME>.git (push)
upstream        https://github.com/BlockLabz/<REPOSITORY_NAME>.git (fetch)
upstream        https://github.com/BlockLabz/<REPOSITORY_NAME>.git (push)
```

### Create a new branch

Create a **branch** to make your contribution:

```bash
$git checkout -b feature/feature_name
```

After completing your contribution, send it to the remote repository in your account:

```bash
$git push origin feature/feature_name
```

### Make a pull request

In your github account, submit a **Pull Request** with your contribution to the official repository:

![image](https://user-images.githubusercontent.com/50463866/103661883-0089b400-4f4e-11eb-8752-3c341fdc3e4a.png)

Now wait for the review from one of the project's maintainers.
