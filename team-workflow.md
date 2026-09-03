# Ticket Defense Team Workflow

## Team Members

* Josiah Rhodes
* Daren Diaz
* JT Russell
* adejayz

Team members will claim responsibilities through assigned GitHub Issues. Each issue should identify the owner, expected result, and acceptance criteria for the task.

## Branching Strategy

Our team will not make routine project changes directly on the `main` branch. The `main` branch should contain only reviewed and working changes. Every task will be completed on a separate branch connected to a GitHub Issue.

Before creating a branch, each team member must switch to `main` and pull the latest changes:

```bash
git switch main
git pull origin main
```

Branch names should be lowercase, use hyphens between words, and describe the purpose of the work.

Branch name examples:

* `feature/create-ticket-enemy`
* `feature/add-score-system`
* `docs/update-readme`
* `fix/ticket-timer-bug`
* `test/add-ticket-tests`

## Pull Request Process

Each completed task must be submitted through a pull request into `main`.

Before opening a pull request, the team member should:

* Confirm they are working on a task branch and not `main`
* Verify that the task has a related GitHub Issue
* Complete only the work described in the issue
* Review the changed files for accidental or unnecessary changes
* Confirm the project still runs or the documentation displays correctly
* Commit the changes with a clear message
* Push the branch to GitHub
* Open a pull request into `main`
* Reference the related issue using `Closes #<issue-number>`
* Request a review from at least one teammate

Pull requests should have a clear title and a short description explaining what changed, why it changed, and how the work was verified.

## Code Review Expectations

At least one teammate other than the author should review each pull request before it is merged. Team members should not merge their own pull requests before receiving approval unless the instructor gives permission.

Reviewers should check:

* Does the change satisfy the related issue and its acceptance criteria?
* Was the work completed on a separate branch?
* Is the code or documentation understandable and organized?
* Are unrelated or unnecessary files included?
* Are there obvious errors, security concerns, or exposed secrets?
* Does the change require tests, and were those tests completed?
* Does the project still build or run as expected?

If changes are requested, the author should make them on the same branch, commit them, and push again. GitHub will automatically update the existing pull request.

## Commit Message Expectations

Commit messages should be short, specific, and clearly explain the change.

Good examples:

* `Create team workflow document`
* `Add team member project contribution`
* `Create initial ticket enemy component`
* `Fix ticket countdown calculation`
* `Add tests for scoring rules`

Weak examples:

* `update`
* `stuff`
* `final`
* `fixed things`
* `changes`

Each commit should focus on one logical change whenever practical. Secrets, passwords, API keys, generated build files, and unrelated personal files must not be committed.

## Issue Tracking

The team will use GitHub Issues to plan and track work. Each issue should include:

* A clear title
* A description of the requested work
* Acceptance criteria explaining when the task is complete
* An assigned team member
* Appropriate labels when available
* A link to the related pull request

Before beginning work, the assigned team member should move the issue to **In Progress**. A pull request should reference its issue with `Closes #<issue-number>` so GitHub can close the issue automatically after the pull request is merged.

## Project Board

The team will use the GitHub Project board to show the current status of project work.

Board columns:

* **Backlog** - Ideas or future work that has not been scheduled
* **To Do** - Approved tasks that are ready to begin
* **In Progress** - Tasks currently being worked on
* **Review** - Completed work awaiting pull-request review
* **Done** - Reviewed and merged work

Team members are responsible for keeping their assigned items current. Issues should move to **Review** when a pull request is opened and to **Done** after the pull request is approved and merged.

## Standard Team Workflow

Every routine task should follow this process:

1. Create or claim a GitHub Issue.
2. Assign the issue and move it to **In Progress**.
3. Switch to `main` and pull the latest changes.
4. Create a clearly named branch for the issue.
5. Make and verify the required changes.
6. Review, stage, and commit the changes.
7. Push the branch to GitHub.
8. Open a pull request and reference the issue.
9. Move the issue to **Review**.
10. Have at least one teammate review the pull request.
11. Address any requested changes on the same branch.
12. Merge the approved pull request into `main`.
13. Delete the merged branch.
14. Confirm the issue is closed and move it to **Done**.

Following this workflow will keep the Ticket Defense repository organized, reduce conflicting changes, and ensure that team contributions are reviewed before becoming part of the main project.
