# git-profile

This project provides a quick and simple way to switch between Git configurations. For example, perhaps you have one `.gitconfig` file that you want to use at work, and one for open source projects to which you contribute when vacationing at your summer home in the Swiss Alps. Switching to your home profile after performing some emergency work for the office is easy:

```
git profile use home
```

Execute `git profile help` for some help. You can see that the `bash_git_profile` script wraps the main Git command. Anything unrelated to Git Profile is just passed through (after reminding you of your current profile).

There's a how-to video available, if you want to see git-profile in action: [Using the git-profile project](https://vimeo.com/175977332)

## Installation

Clone the project repo. Perhaps, `cd ~/Projects; git clone git@github.com:jlamoree/git-profile.git`.

### Update your Bash login profile

Update `~/.bash_profile` to source the Bash script. For example, `source ~/Projects/git-profile/bash_git_profile`.

Check out the configuration options in the top of the Bash script.

### Profiles Path

The `GIT_PROFILES_PATH` variable points to your profiles, as you might guess. This could be something like `$HOME/.gitprofiles` or `$HOME/Dropbox/GitProfiles` if you want to sync your profiles.

### Profile Reminder

The `GIT_PROFILE_REMINDER` variable controls whether you want to be reminded of your current profile when running any Git commands. The default is "yes".

## Bugs/Enhancements

Please use [GitHub Issues](https://github.com/jlamoree/git-profile/issues) to provide feedback.

## License

This project uses the MIT License.
