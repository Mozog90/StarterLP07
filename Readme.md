# Learning Practice: Test Planning

## Topics

- Test objectives and scope
- Test approach
- Roles and responsibilities
- Test environments and test data
- Risks and mitigation
- Entry and exit criteria
- Test schedules and communication

## Learning Objectives

- Explain the purpose of a test plan.
- Define the scope and objectives of testing.
- Select appropriate test types and techniques.
- Identify the people, tools, environments, and data needed for testing.
- Identify testing risks and possible responses.
- Create measurable entry and exit criteria.
- Organize testing activities into a simple schedule.

## The Product

The North Vacation Booking development team is preparing a new version of its booking application.

The application allows a user to:

- Select a rental.
- Enter check-in and checkout dates.
- Enter the number of guests.
- Create a booking.
- View their bookings.
- Increase, decrease, or reset values where applicable.

The team wants a plan describing how the application should be tested before release. You will create a short test plan for this release.

## Step 1: Define the Test Context

Describe what will be tested and why.

Include:

- Two test objectives
- Features that are in scope
- Features that are out of scope
- The test basis, such as requirements, user stories, source code, or designs
- At least one assumption or constraint

<details>
<summary>Example format</summary>

| Section                  | Description                                   |
| ------------------------ | --------------------------------------------- |
| Test objective           | Confirm that users can create a valid booking |
| In scope                 | Booking form and booking list                 |
| Out of scope             | Payment processing                            |
| Test basis               | Booking requirements and user stories         |
| Assumption or constraint | Testing must be completed within one week     |

</details>

## Step 2: Identify Roles and Responsibilities

Identify at least **three roles** involved in testing.

For each role, explain:

- What the person is responsible for
- When they will be involved
- Who they need to communicate with

<details>
<summary>Example format</summary>

| Role   | Responsibilities           | When Involved                    | Communication                 |
| ------ | -------------------------- | -------------------------------- | ----------------------------- |
| Tester | Designs and executes tests | Before and during test execution | Reports defects to developers |
|        |                            |                                  |                               |

</details>

## Step 3: Define the Test Approach

Explain how the application will be tested.

Include:

- The test levels that will be used
- At least two test types
- At least two test techniques
- Any manual or automated testing
- The test deliverables that will be created

Possible test deliverables include:

- Test cases
- Automated test files
- Test results
- Coverage reports
- Defect reports
- A test completion report

<details>
<summary>Example format</summary>

| Test Area    | Test Level or Type | Technique               | Manual or Automated | Deliverable    |
| ------------ | ------------------ | ----------------------- | ------------------- | -------------- |
| Booking form | Component testing  | Boundary value analysis | Automated           | Jest test file |
|              |                    |                         |                     |                |

</details>

## Step 4: Identify Test Requirements

Describe what is needed to complete the testing.

Include:

- The test environment
- Browsers or devices
- Testing tools
- Test data
- Any access, accounts, or permissions
- Any people or training needed

## Step 5: Create a Risk Register

Identify at least **three risks** that could affect the product or the testing process.

For each risk, include:

- A description of the risk
- Whether it is a product risk or project risk
- Its likelihood
- Its impact
- A possible mitigation

<details>
<summary>Example risk register</summary>

| Risk                                           | Type         | Likelihood | Impact | Mitigation                           |
| ---------------------------------------------- | ------------ | ---------- | ------ | ------------------------------------ |
| A user can create a booking with invalid dates | Product risk | Medium     | High   | Prioritize date validation tests     |
| The test environment is unavailable            | Project risk | Low        | High   | Confirm access before testing begins |
|                                                |              |            |        |                                      |

</details>

## Step 6: Define Entry Criteria

Entry criteria describe what must be ready before test execution can begin.

Create at least **three entry criteria** for this project.

Your criteria may address:

- Availability of testable code
- Completion of earlier testing
- Availability of the test environment
- Availability of test cases
- Availability of test data
- Installation of testing tools

Write criteria that can be clearly checked as met or not met.

## Step 7: Define Exit Criteria

Exit criteria describe when testing is complete or when it should stop.

Create at least **three measurable exit criteria**.

Your criteria may address:

- Percentage of planned tests completed
- Required code or requirements coverage
- Number or severity of unresolved defects
- Completion of high-risk testing
- Successful regression testing
- Release deadlines

<details>
<summary>Example entry and exit criteria table</summary>

| Type  | Criterion                                             |
| ----- | ----------------------------------------------------- |
| Entry | The application can be opened in the test environment |
| Entry | All planned test cases have been reviewed             |
| Exit  | All planned high-priority tests have been executed    |
| Exit  | No critical defects remain unresolved                 |

</details>

## Step 8: Create a Test Schedule

Create a simple schedule containing at least **five testing activities**.

Include:

- The activity
- The person or role responsible
- When it will happen
- Any activity that must be completed first

<details>
<summary>Example schedule</summary>

| Activity            | Responsible Role         | Time  | Dependency                      |
| ------------------- | ------------------------ | ----- | ------------------------------- |
| Review requirements | Tester and product owner | Day 1 | Requirements are available      |
| Design test cases   | Tester                   | Day 2 | Requirements have been reviewed |
|                     |                          |       |                                 |

</details>

## Step 9: Define the Communication Plan

Explain how testing information will be shared with the team.

Include:

- What information will be communicated
- Who will receive it
- How it will be communicated
- When or how often it will be communicated

<details>
<summary>Example communication plan</summary>

| Information   | Audience     | Method         | Frequency              |
| ------------- | ------------ | -------------- | ---------------------- |
| Test progress | Project team | Daily stand-up | Daily                  |
| Defect report | Developer    | GitHub issue   | When a defect is found |
|               |              |                |                        |

</details>

## What to Submit

1. Create and initialize a GitHub repository.
2. Commit and push your work to the repository.
3. Make sure the repository is public. Private repositories will not receive credit.
4. Submit the URL on canvas

## AI Transparency

AI was used to help create portions of this file and to clean up its writing and formatting.

## 1. Test Context

**Purpose:** This test plan explains how I would test the next release of the North Vacation Booking application before it goes live.

**Test objectives**

1. Verify that users can create bookings with valid rental, date, and guest information, and that invalid information is handled correctly.
2. Verify that users can view their bookings and that any increase, decrease, or reset controls work as expected.

**In scope**

- Selecting a rental
- Entering check-in and checkout dates
- Entering the number of guests
- Creating a booking
- Viewing the booking list
- Increase, decrease, and reset controls, where available
- Validation and error messages for the above features

**Out of scope**

- Payments and refunds
- Cancellations
- Account registration and login
- Features that are not included in this release

**Test basis:** The provided application description, booking requirements, user stories, and any available designs or source code.

**Assumption/constraint:** I am planning for five working days of testing. I am also assuming a working test environment and sample rentals will be available. Exact date and guest limits will need to come from the requirements before those tests are finalized.

## 2. Roles and Responsibilities

| Role          | Responsibilities                                                | When Involved                                  | Communication                                   |
| ------------- | --------------------------------------------------------------- | ---------------------------------------------- | ----------------------------------------------- |
| Tester        | Write test cases, run tests, record results, and report bugs    | Throughout testing                             | Works with developers and the product owner     |
| Developer     | Fix defects, review bug reports, and support retesting          | During preparation and whenever bugs are found | Communicates fixes to the tester                |
| Product Owner | Clarify expected behavior, priorities, and release requirements | Before testing and during release review       | Answers questions from the tester and developer |

## 3. Test Approach

| Test Area                              | Level / Type             | Technique                            | Manual or Automated                                   | Deliverable                    |
| -------------------------------------- | ------------------------ | ------------------------------------ | ----------------------------------------------------- | ------------------------------ |
| Date and guest inputs                  | Component / functional   | Boundary value analysis              | Manual initially; automated if test code is available | Input validation test cases    |
| Booking creation                       | Integration / functional | Equivalence partitioning             | Manual                                                | Booking test cases and results |
| Viewing bookings                       | System / functional      | Scenario-based testing               | Manual                                                | End-to-end test results        |
| Increase, decrease, and reset controls | Component / regression   | Boundary value analysis              | Manual initially; automated if practical              | Control test cases             |
| Previously working booking features    | System / regression      | Retesting and scenario-based testing | Manual                                                | Regression results             |

I would test valid and invalid inputs, including a checkout date before the check-in date, empty required fields, and guest counts at the allowed limits. For equivalence partitioning, I would group inputs into valid and invalid sets instead of testing every possible value. I would then complete a full booking from rental selection to checking that it appears in the booking list.

**Test deliverables:** Test cases, recorded pass/fail results, defect reports, and a short test completion summary. If automated tests are added, I would also include the test files and their results.

## 4. Test Requirements

| Requirement        | What Is Needed                                                                                                                      |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------- |
| Test environment   | A working test version of North Vacation Booking with sample rentals                                                                |
| Browsers / devices | A Windows desktop using Chrome and Edge                                                                                             |
| Tools              | Browser developer tools, a test-case checklist, and GitHub Issues for tracking bugs                                                 |
| Test data          | Sample rentals, valid and invalid dates, and guest counts including boundary values                                                 |
| Access             | Permission to use the test environment and create/view sample bookings                                                              |
| People / training  | A developer to answer technical questions and a product owner to clarify requirements; basic instructions for using the application |

## 5. Risk Register

| Risk                                                          | Type    | Likelihood | Impact | Mitigation                                                                 |
| ------------------------------------------------------------- | ------- | ---------- | ------ | -------------------------------------------------------------------------- |
| The application accepts invalid booking dates                 | Product | Medium     | High   | Prioritize date validation and boundary tests                              |
| A booking is created but does not show up in the booking list | Product | Medium     | High   | Verify the full create-and-view workflow                                   |
| The test environment is unavailable                           | Project | Medium     | High   | Confirm access on Day 1 and report downtime immediately                    |
| Requirements for guest limits or controls are unclear         | Project | Medium     | Medium | Ask the product owner to clarify expected behavior before finalizing tests |

## 6. Entry Criteria

Testing can begin when all of the following are met:

1. The test version of the application opens successfully in the test environment.
2. The rental selection, booking form, and booking list are available to test.
3. Sample rentals and the required test data are ready.
4. The planned test cases have been written and reviewed.

## 7. Exit Criteria

Testing is considered complete when all of the following are met:

1. **100%** of planned test cases have been executed.
2. At least **95%** of test cases pass, and any remaining failures are documented.
3. **Zero critical or high-severity defects** remain unresolved.
4. All high-priority booking scenarios and regression tests pass.

If these criteria are not met by the end of Day 5, I would report the remaining issues and recommend whether the release should be delayed.

## 8. Test Schedule

| Activity                                          | Responsible Role         | When  | Dependency                           |
| ------------------------------------------------- | ------------------------ | ----- | ------------------------------------ |
| Review requirements and confirm expected behavior | Tester and product owner | Day 1 | Requirements are available           |
| Prepare test environment and sample data          | Tester and developer     | Day 1 | Test build is available              |
| Write and review test cases                       | Tester                   | Day 2 | Requirements have been reviewed      |
| Execute functional and boundary tests             | Tester                   | Day 3 | Test cases and environment are ready |
| Report defects and retest fixes                   | Tester and developer     | Day 4 | Initial tests have been run          |
| Run regression tests and write completion summary | Tester                   | Day 5 | Fixes and retesting are complete     |

## 9. Communication Plan

| Information                        | Audience                    | Method                  | When                             |
| ---------------------------------- | --------------------------- | ----------------------- | -------------------------------- |
| Test progress and blockers         | Developer and product owner | Short team update       | Daily during testing             |
| New bugs and steps to reproduce    | Developer                   | GitHub Issue            | As soon as a defect is found     |
| Questions about expected behavior  | Product owner               | Team chat or meeting    | Whenever clarification is needed |
| Test results and release readiness | Whole team                  | Test completion summary | End of Day 5                     |

## Summary

This plan focuses on making sure users can select a rental, enter booking details, create a booking, and see it afterward. I would prioritize date validation and the main booking workflow because problems there could prevent users from making reservations. The test results and any remaining defects would be shared with the team before the release decision.
