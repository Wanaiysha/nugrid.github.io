# Developer Guide
In this document we collect best practices and guidlines for NuGrid code developements. 



## General rules
1. Any information must only be maintained in one place, using appropriate referencing as needed.

## Git repositories
Git and our remote GitHub offer (and sometimes impose) good techniques for collaborative software developement. 

### General rules
1. github issues are not a discussion forum, use slack or nugrid-team instead
2. pull requests are not the discussion forum for ongoing development, but meant to be leading in the short term
   to a merge
3. general advise: try to merge often, chunk up work into manageable pieces



### Code improvements and bug fixes: branching and merging
Improving the code (enhancement of bug fixes) are a common activity. The following steps describe the procedure:

1. If you want to implement anything new in the master you start by creating a branch on your own local repo.
2. Develop your branch for a bit. This typically involves a number of `git add` and `git commit` cycles. At any time you can push the branch back to the remote, now everybody can see the branch, and can provide help working on this particular branch.
3. To ask for and coordinate help you can issue an _issue_, use _slack_ or write an _email to nugrid-team_.
4. As developement on your branch proceeds you will do the regression testing that is beeing put in place.
5. Finally you (and your team) think you have something that should go back to the master; this is when you put in a pull request. In the description of the pull request you may _mention_ collaborators who should take note. For example, this is how I mention `@marcop`. You can also mention issues, such as issue `#21`. Try it. Mentions will notify those who have been mentioned (depending how they have configured their github). In addition you will assign _assignees_. Those are the gatekeepers who have to agree for admitting the pull request. The assignees will be listed by github in alpha-numeric order, so you can not suggest a primary and then some secondary assignees. Therefore **all assignees leave a message in the pull request comment section indicating their sign-off, and whoever is last will push the button.** [This is not ideal, but it seems github does not provide a better mechanism for this.]
6. After the merge the person who has created the branch may decide that the branch be deleted or it just stays their, no harm done. However, there is no reason to leave it there unless more development continues on this branch, so as a general rule merged branches should be deleted.
