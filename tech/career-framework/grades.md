# Grades

The last piece of the puzzle is grading within career tracks. Career progress is a continuous number between 0 and 5, however we need to establish a finite number of job titles, grades in company-wide career ladder etc. That is why each career track is subdivided into finite (usually 4) buckets. **Based on your career track and progress, you can look up your grade within the table below.** That will determine your job title, your minimum salary bound, next salary bound and also grade in company-wide career ladder. It contains the following columns:

- **Career Track** - Name of the [career track](career-tracks/readme.md).
- **Min P** - Minimum [progress](progress.md) in the [career track](career-tracks/readme.md) required for the grade. Closed lower bound.
- **Max P** - Maximum [progress](progress.md) in the [career track](career-tracks/readme.md) required for the grade. Open upper bound.
- **Grade** - Grade within the company-wide career ladder.
- **Job Title** - Job title corresponding to the grade and career track.
- **Min Salary** - Minimum normalized salary awarded to the grade and career track.
- **Next Salary** - Next minimum normalized salary, corresponding to max progress.

> Please note that currently, we are not publishing the salary columns, those have been redacted out. All the examples involving salaries in these guides are arbitrary and do not represent reality.

For example an engineer with progress P = 2.50 would have grade IC4, minimum normalized salary 80000 and next normalized salary 120000. Their job title would be e.g. "Senior Backend Engineer". Some job titles contain `{Discriminator}` which is a dynamic placeholder that can be replaced with various values, most common ones are "Backend", "Frontend" and "Mobile" in case of IC roles. For management roles, it can be name of family or division. More on how to interpret and work with the normalized salaries can be found in the [compensation](compensation.md) guide.

| Career Track               | Min P | Max P | Grade | Job Title                                       | Min Salary | Next Salary |
|----------------------------|-------|-------|-------|-------------------------------------------------|------------|-------------|
| Product Division Lead      | 3.50  | 5.00  | L1    | VP Engineering, Product                         |            |             |
| Platform Division Lead     | 3.50  | 5.00  | L1    | VP Engineering, Platform                        |            |             |
| Product Family Lead        | 0.00  | 2.00  | S2    | Engineering Manager, {Discriminator}            |            |             |
| Product Family Lead        | 2.00  | 3.10  | M1    | Engineering Manager, {Discriminator}            |            |             |
| Product Family Lead        | 3.10  | 4.20  | D1    | Director of Engineering, {Discriminator}        |            |             |
| Product Family Lead        | 4.20  | 5.00  | D2    | Senior Director of Engineering, {Discriminator} |            |             |
| Platform Family Lead       | 0.00  | 2.00  | S2    | Engineering Manager, {Discriminator}            |            |             |
| Platform Family Lead       | 2.00  | 3.10  | M1    | Engineering Manager, {Discriminator}            |            |             |
| Platform Family Lead       | 3.10  | 4.20  | D1    | Director of Engineering, {Discriminator}        |            |             |
| Platform Family Lead       | 4.20  | 5.00  | D2    | Senior Director of Engineering, {Discriminator} |            |             |
| Product Team Lead          | 0.00  | 1.40  | S1    | Engineering Manager                             |            |             |
| Product Team Lead          | 1.40  | 2.60  | S2    | Engineering Manager                             |            |             |
| Product Team Lead          | 2.60  | 3.80  | M1    | Engineering Manager                             |            |             |
| Product Team Lead          | 3.80  | 5.00  | M2    | Senior Engineering Manager                      |            |             |
| Platform Team Lead         | 0.00  | 1.40  | S1    | Engineering Manager                             |            |             |
| Platform Team Lead         | 1.40  | 2.60  | S2    | Engineering Manager                             |            |             |
| Platform Team Lead         | 2.60  | 3.80  | M1    | Engineering Manager                             |            |             |
| Platform Team Lead         | 3.80  | 5.00  | M2    | Senior Engineering Manager                      |            |             |
| IT and Security Lead       | 0.00  | 1.40  | S1    | IT and Security Manager                         |            |             |
| IT and Security Lead       | 1.40  | 2.60  | S2    | IT and Security Manager                         |            |             |
| IT and Security Lead       | 2.60  | 3.80  | M1    | IT and Security Manager                         |            |             |
| IT and Security Lead       | 3.80  | 5.00  | M2    | Senior IT and Security Manager                  |            |             |
| Technical Leader           | 0.00  | 3.80  | IC4   | Staff {Discriminator} Engineer                  |            |             |
| Technical Leader           | 3.80  | 4.40  | IC5   | Senior Staff {Discriminator} Engineer           |            |             |
| Technical Leader           | 4.40  | 5.00  | IC5   | Principal {Discriminator} Engineer              |            |             |
| Agile Coach                | 0.00  | 1.40  | IC2   | Agile Coach                                     |            |             |
| Agile Coach                | 1.40  | 2.60  | IC3   | Agile Coach                                     |            |             |
| Agile Coach                | 2.60  | 3.80  | IC4   | Senior Agile Coach                              |            |             |
| Agile Coach                | 3.80  | 5.00  | IC5   | Staff Agile Coach                               |            |             |
| Community Manager          | 0.00  | 1.40  | S1    | Community Manager                               |            |             |
| Community Manager          | 1.40  | 2.60  | S2    | Community Manager                               |            |             |
| Community Manager          | 2.60  | 3.80  | M1    | Community Manager                               |            |             |
| Community Manager          | 3.80  | 5.00  | M2    | Senior Community Manager                        |            |             |
| Engineer                   | 0.00  | 1.20  | IC2   | {Discriminator} Engineer                        |            |             |
| Engineer                   | 1.20  | 2.40  | IC3   | {Discriminator} Engineer                        |            |             |
| Engineer                   | 2.40  | 3.60  | IC4   | Senior {Discriminator} Engineer                 |            |             |
| Engineer                   | 3.60  | 5.00  | IC5   | Staff {Discriminator} Engineer                  |            |             |
| Data Scientist             | 0.00  | 1.20  | IC2   | Data Scientist                                  |            |             |
| Data Scientist             | 1.20  | 2.40  | IC3   | Data Scientist                                  |            |             |
| Data Scientist             | 2.40  | 3.60  | IC4   | Senior Data Scientist                           |            |             |
| Data Scientist             | 3.60  | 5.00  | IC5   | Staff Data Scientist                            |            |             |
| Product Security Engineer  | 0.00  | 1.20  | IC2   | Product Security Engineer                       |            |             |
| Product Security Engineer  | 1.20  | 2.40  | IC3   | Product Security Engineer                       |            |             |
| Product Security Engineer  | 2.40  | 3.60  | IC4   | Senior Product Security Engineer                |            |             |
| Product Security Engineer  | 3.60  | 5.00  | IC5   | Staff Product Security Engineer                 |            |             |
| IT Security Engineer       | 0.00  | 1.20  | IC2   | IT Security Engineer                            |            |             |
| IT Security Engineer       | 1.20  | 2.40  | IC3   | IT Security Engineer                            |            |             |
| IT Security Engineer       | 2.40  | 3.60  | IC4   | Senior IT Security Engineer                     |            |             |
| IT Security Engineer       | 3.60  | 5.00  | IC5   | Staff IT Security Engineer                      |            |             |
| Data Analyst               | 0.00  | 1.20  | IC2   | Data Analyst                                    |            |             |
| Data Analyst               | 1.20  | 2.40  | IC3   | Data Analyst                                    |            |             |
| Data Analyst               | 2.40  | 3.60  | IC4   | Senior Data Analyst                             |            |             |
| Data Analyst               | 3.60  | 5.00  | IC5   | Staff Data Analyst                              |            |             |
| IT Infrastructure Engineer | 0.00  | 1.20  | IC2   | IT Infrastructure Engineer                      |            |             |
| IT Infrastructure Engineer | 1.20  | 2.40  | IC3   | IT Infrastructure Engineer                      |            |             |
| IT Infrastructure Engineer | 2.40  | 3.60  | IC4   | Senior IT Infrastructure Engineer               |            |             |
| IT Infrastructure Engineer | 3.60  | 5.00  | IC5   | Staff IT Infrastructure Engineer                |            |             |
| QA Engineer                | 0.00  | 1.20  | IC1   | QA Engineer                                     |            |             |
| QA Engineer                | 1.20  | 2.40  | IC2   | QA Engineer                                     |            |             |
| QA Engineer                | 2.40  | 3.60  | IC3   | Senior QA Engineer                              |            |             |
| QA Engineer                | 3.60  | 5.00  | IC4   | Staff QA Engineer                               |            |             |
| IT Specialist              | 0.00  | 1.20  | IC1   | IT Specialist                                   |            |             |
| IT Specialist              | 1.20  | 2.40  | IC2   | IT Specialist                                   |            |             |
| IT Specialist              | 2.40  | 3.60  | IC3   | IT Specialist                                   |            |             |
| IT Specialist              | 3.60  | 5.00  | IC4   | Senior IT Specialist                            |            |             |
| Community Coordinator      | 0.00  | 1.20  | IC1   | Community Coordinator                           |            |             |
| Community Coordinator      | 1.20  | 2.40  | IC2   | Community Coordinator                           |            |             |
| Community Coordinator      | 2.40  | 3.60  | IC3   | Community Coordinator                           |            |             |
| Community Coordinator      | 3.60  | 5.00  | IC4   | Senior Community Coordinator                    |            |             |
