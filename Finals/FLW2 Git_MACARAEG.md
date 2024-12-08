![image](https://github.com/user-attachments/assets/acd8afa2-a9a4-40e9-9258-9d66e28ddac0)

# SYSADM1 – Git Basics
Answer the following research questions about Git, GitLab desktop and GitHub.

1. What is Git, and why is it important in software development?

   |- Git is a distributed version control system that tracks changes in code and allows multiple developers to collaborate efficiently. It is crucial in software development as it helps manage code versions, prevent overwriting, and enables seamless collaboration among teams.|
   | :- |

1. How does Git track changes in a project?

   |- Git tracks changes using snapshots. Each commit represents a snapshot of the project’s file at a specific point. Git compares differences between these snapshots and store only the changes, making the process efficient.|
   | :- |

1. What is the difference between a local repository and a remote repository in Git?

   |- A loca repository resides on a developer’s computer and allows for offline work. A remote repository is hosted on a server, such as GitHub or GitLab, enabling collaboration and centralized code management.|
   | :- |

1. What are the basic Git commands? 

   |<p>- ***git init***   = Initialize a repository</p><p>- ***git clone***   = Clone a remote repository</p><p>- ***git add***   = Stage changes for a commit</p><p>- ***git commit***  = Save changes to the local repository</p><p>- ***git push***   = Upload local changes to the remote repository</p><p>- ***git pull***   = Fetch and merge changes from a remote repository</p><p>- ***git status***   = Check the repository’s status</p>|
   | :- |

1. How do you check the status of a Git repository? 

   |- Use the command ***git status*** it shows the current state of the repository.***  |
   | :- |

1. What is the purpose of branches in Git, and how do you create and switch between them?

   |<p>- Branches allow developers to work on different features or fixes simultaneously without affecting the main codebase.</p><p>- ***git branch branch\_name***. To create a branch:</p><p>- ***git checkout branch\_name or git switch branch\_name.*** To switch branches </p>|
   | :- |

1. What are GitLab Desktop and GitHub, and how are they different from Git?

   |- GitLab Desktop and GitHub are platforms for hosting Git repositories. They provide additional tools for collaboration, issue tracking, and CI/CD. Git, on the other hand, is the underlying version control system used for tracking changes.|
   | :- |

1. How do you connect a local Git repository to a GitLab or GitHub repository?

   |<p>- Create a repository on GitLab or GitHub.</p><p>- In your local project, add the remote repository using: ***git remote add origin <repository\_url>***</p><p>- Push your code with:  ***git –u origin branch\_name***</p>|
   | :- |

1. What are the steps to collaborate with others using GitLab or GitHub?	

   |<p>- Clone the remote repository: ***git clone <repository\_url>.***</p><p>- Create a branch for your changes.</p><p>- Make and commit changes.</p><p>- Push the branch to the remote repository.</p><p>- Open a pull or merge request for review.</p><p>- Resolve any feedback or merge conflicts, then merge the branch.</p>|
   | :- |

1. How do you resolve merge conflicts in Git?

   |<p>- Identify the conflict with ***git status.***</p><p>- Open the conflicting files and manually resolve the conflicts.</p><p>- Stage the resolved files using ***git add.***</p><p>- Complete the merge with ***git commit.***</p>|
   | :- |

1. What is a pull request, and why is it used in GitHub?

   |- A pull request (PR) is a way to propose changes in codebase. It allows developers to review, discuss, and approve changes before merging them into the main branch, ensuring quality and collaboration.|
   | :- |

1. What are some best practices for writing commit messages?

   |<p>- Use a clear and concise subject line (50 characters max).</p><p>- Write in the imperative mood (e.g., "Add feature" instead of "Added feature").</p><p>- Include a detailed description if necessary.</p><p>- Focus on what was changed and why, rather than how it was done.	</p>|
   | :- |

`	`Page 2** of 2**	
