# BIT 300: Get-Set Mobile Github and Android Studio
## GIT basics and Best Practices

1. Why Git?

   * There are other version control systems. There are a number of Version Control Systems out there. This alone should prove that version control is incredibly important. Examples are   [Git](https://git-scm.com), [Subversion](https://subversion.apache.org) and [Mercurial](https://www.mercurial-scm.org)

    * Git is the most popular and an industry standard.

   * It has some advantages over a centralized system, which has a single copy of the code:

     * It's quick to take action on your own copy WHICH IS GREAT!
     * It works locally, on your own computer, and offline
     * It makes having multiple branches, parallel worlds of code, easier

     ![git workflow steps](./GitWorkFlow.gif)

2. Git Gotchas

   * Git can mean several things - the name of the source control technology, the functionality built into VS Code, the file formats and protocols that underlie the system.
   * It’s both powerful (because it’s open-ended), plentiful (because it’s open source), and sometimes hard to use (because it’s open-ended).
   * It takes practice, it's a learned skill, it's not intuitive - ask other developers about their Git disasters - everyone has a story.


## Git Demo Using Git Bash/ Android Studio Terminal

1. Creating new repo and initial commit. The flow for using git starts with creating a directory (folder). The cycle as changes are made is `add` and `commit`. Record your changes in small chunks as you go.

   * Configure your git
     * `git config --global user.email "youremail"`
     * `git config --global user.name "yourname"`
   * `mkdir SampleApp` - create new folder named SampleApp
   * `cd SampleApp` - move to the project folder
   * `git init` - initialize the repository
   * `touch README.md` - create a new file
   * `git status` - view the repository status
   * `git add  .` - stage the files to commit and tell get what files to track, "." selects all the new files or files with changes
   * `git commit README.md -m "New readme file"` - add the changes to the repo with the named file, "-m" indicates message included


## Demo: Git using Android Studio's VCS menu

1. Create a new "Empty Activity" project in Android Studio and use the built-in git support (*VCS menu*). It doesn't have all the commands of Git Bash or the command line but is convenient when working in Android Studio.

2. Add a TEXT file with a distinctive name (File/New/File)

3. Use "*VCS > Enable Version Control Integration*" to initialize a repository - choose "Git" as your VCS

4. Follow the git workflow 

   * **View the repository status**: using "*Git>Commit*" from the menu
   * **Stage the files to commit**: select the file you created from the list (find it in the *Unversioned Files* list)
   * **Commit the changes with a comment**: Type a commit message in the box, like "tests commit process in Android Studio" and click "Commit"

5. Review the effect using the Terminal

   * Open the "Terminal" tab "*View > Tool Windows > Terminal*"
   * Check out the changes with `git log`
   * See the difference between `git log` and `git log --oneline`

## Work with Remote GitHub repositories
### use the Canvas document to complete the exercise with a programming partner
1. The person in your team with a GitHub account should "drive" first
2. **Fork** (button in upper-left corner of) THIS GitHub repository to create a new copy in YOUR GitHub account
3. Open Android Studio; use the menu option "*File > New > Project from Version Control*" with your GitHub URL
4. Each person in your group should make at least two commits as shown above; use both the Android Studio terminal and Android Studio VCS to work with Git
5. Push your changes to GitHub using the Android Studio "*Git > PUSH*" menu or the terminal command `git push`

## Submission (one per group )
Submit the URL for the updated GitHub repository in Canvas
One per group meaning one submission will be used to grade both people.

This means sometimes you will only use one computer/laptop This is the end 
