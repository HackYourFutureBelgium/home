# Homework Feedback

> check out `../students/hyf-workflows/module-projects` to read about projects
> in their guidebook.

There will be two types of project in the class repo:

- **`individual`**: Individual projects will have the `individual` label
- **`group`**: On weeks where there is a group project each study group will
  create only one issue for their project.

## Module Project Board

There will be a project board to keep track of all the group projects in your
module. The columns you'll care most about are **Doing** and **Ready For
Review**

Groups will add the `help-wanted` label to their issues in the _Doing_ columns
when they are blocked. If they don't explain why they are blocked in their issue
you can ask for specifics before looking through their repo. You don't need to
dig through all their project repo to figure out what is blocking them.

Issues in **Ready for Review** are, well, ready for review.

### Move to DONE if ...

- They have a good Retrospective
- All the check-boxes are completed and the links work
- They have a well-organized project board
- Issues and pull requests are linked appropriately
- The backlog and development strategy files shows clear planning \(even if it
  doesn't line up with what the final issues/branches, or their actual project
  has changed from what they planned\)

### Move to NEEDS REVISION if ...

- any of the checklist links are dead or don't go to the right place. You're
  here to give a code review, not to dig through their github accounts
- the student still has a `help-wanted` label on their issue
- there are validation errors or failing tests in the project \(not all projects
  will have tests or validation\)
- the project planning is way off from what they actually built. In this case
  you can ask them to update the file to match what they did develop in their
  repo, instead of asking them to redevelop the project.

## Giving Feedback

Here are some thumb rules on giving feedback.

### Something is better than nothing

- Getting any amount of feedback is one of the most helpful things we can do for
  students, at least as helpful as Sunday classes.
- It's better to give enough good feedback to more students than lots of great
  feedback to fewer students.
- Give at least two pieces of feedback to each student in the group you review:
  1 thing they did well, 1 thing they can improve. This could be about their
  code, about how their code reviews, their design, their communication skills
  ... anything you noticed.

### Open Communication

- If you can’t review on time let students know. Either individually or in the
  class channel.
- Same thing if you'll be late reviewing the assignments. Just a short
  Slack-message or comment on their group issue is enough.
- Be open and clear about your review criteria. It can be very demotivating for
  students to get very different feedback on the same level of work.
- If you do give different levels of feedback to different students, let them
  know why.

### What/How to give feedback

- Start with a quick high level check \(links to project, end result,
  validators, etc.\) and ask for corrections \(move the card to _Needs
  Revision_\) before diving into the code.
- Test the solution. First review the bugs you notice in the code.
- Show don’t tell. Include code snippets explaining mistakes.
- Nothing is out of bounds. Feel free to comment on code style, design, their
  README, or whatever you notice that you think would help them.

#### Group Projects

- Prefer to leave general feedback on group projects as a comment in the `group`
  issue so feedback is visible to all groups.
- If you have specific tips for the student to improve the quality of their
  code, that can go as PRs/issues in their group project repo.

#### Individual Exercises

> while not required, it is very nice for the students to receive feedback on
> their `individual` issues

- Prefer to comment on their homework issue in the class repo rather than
  opening an issue on the exercise repo itself, to keep it simple and visible.
- If you do think a PR/code-review in their exercise repository is necessary,
  still write a summary of your review in their homework issue and link to the
  PR.

### Be Motivating

- Add a positive remark, even if there are bugs.
- Add Emoji’s and images to a review. A big block of text is intimidating.
  :fearful:
- For students that are doing well: Give them positive feedback and a more
  advanced assignment \(for example: look for parts that can be refactored using
  a different approach, or a new language feature\)

### Don't be Demotivating. Don't:

- Suggest \(intentionally or not\) that some people are natural programmers and
  some are not.

  Studies have shown that this is not the case. This is sometimes called fixed
  mindset vs growth mindset.

- Do stereotype threat or microaggressions: reminding people about negative
  stereotypes can make them anxious about the risk of confirming those
  stereotypes.

  We try to be inclusive in class and in our examples and exercises.

- Show a contemptuous attitude: treating other people or things as lesser or
  worthless.

  A common pitfall is the word “just” \(e.g. “just install this package”, ”just
  use this pattern”\)

- Comment/joke about other technologies, e.g. Unix vs Windows, vim vs emacs,
  other programming languages vs JavaScript.

  The students are more likely to interpret these literally, applying the
  negativity to themselves or others.

### Do Involve Other Students

- Linking to a classmate's assignment who already fixed the same mistake is a
  good way for them to learn from each other. And it's probably easier than
  explaining the solution yourself :wink:
- If you've seen a strong & helpful student do well on something that another is
  struggling with, go ahead and assign them to help. Mention them in a comment
  describing the problem and assign them to the issue.

### Always be Preppin!

- Write down the common mistakes throughout the homework and review them on
  Wednesday and/or Sunday.
- Cloning and reviewing in a code editor gives you a better feel for the
  students levels. This will help you prepare for Wednesdays and Sundays.

## Acknowledgments

Big thank you's for the contributions and resources:

- [CodeYourFuture](https://teachertraining.codeyourfuture.io/content/motivation-and-demotivation)
- [Tiago](https://github.com/otagi)
- [Teach Together](https://teachtogether.tech)
