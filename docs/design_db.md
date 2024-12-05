WorkSpace: user belong to workspace with difference role, each workspace have difference setting

## Team
- name:
- member:ref to user
- Role: enum value[admin, user]

## Milestone:
- Milestone: title, descriptin, date

## Project:
- Status
- Priority
- Leader
- Team: multiple teams
- Targeted at
- Started at
- Created at
- Updated at
- Short description
- Description
- Milestone: ref list milestones

## SlugHistories
- Slug:
- Team:ref

## Tasks:
- Slug: ref:slug_history:have_one
- Status: Backlog, Active(Todo, Doing, LocalDone, Done, Archive)
- Assignee: ref User, team members
- Creator: ref User, team members (admin role, manage role)
- Priority: (No, Low, Medium, High, Urgent)
- Label: User self create, string
- Project: ref to Project
- Parent issue: self ref to Task
- Sub issues: have many sub issues self-ref
- Blocked issues:
- Blocking issues:
- Issues with references:
-----
- Due date
- Created date
- Updated date
- Started date
- Completed date
- Triaged date
-----
- Subscriber
- AddedLinks
- Template
- creating_status: (Draft, Created, Deleted)
- Team:ref
- index(team, TaskId)

## Status:
- Title
- Description
- Team:ref

## Label:
- ColorCode
- Title
- Team:ref



## favorite tasks:
- task: ref tasks
- user: ref user id
- sort order
- folder: favorite task belong to folder

## Folder:
- Title
- Status: open, closed
