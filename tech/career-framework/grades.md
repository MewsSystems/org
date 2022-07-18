# Grades

The last piece of the puzzle is grading within career tracks. Career progress is a continuous number between 0 and 5, however we need to establish a finite number of job titles, grades in company-wide career ladder etc. That is why each career track is subdivided into finite (usually 4) buckets. **Based on your career track and progress, you can look up your grade within the table below.** That will determine your job title, your minimum salary bound, next salary bound and also grade in company-wide career ladder. It contains the following columns:

- **Career Track** - Name of the [career track](career-tracks/readme.md).
- **Min P** - Minimum [progress](progress.md) in the [career track](career-tracks/readme.md) required for the grade. Closed lower bound.
- **Max P** - Maximum [progress](progress.md) in the [career track](career-tracks/readme.md) required for the grade. Open upper bound.
- **Grade** - Grade within the company-wide career ladder.
- **Job Title** - Job title corresponding to the grade and career track.
- **Min Salary** - Minimum normalized salary awarded to the grade and career track.
- **Next Salary** - Next minimum normalized salary, corresponding to max progress.

For example an engineer with progress P = 2.50 would have grade IC4, minimum normalized salary 98000 and next normalized salary 138000. Their job title would be e.g. "Senior Backend Engineer". Some job titles contain `{Discriminator}` which is a dynamic placeholder that can be replaced with various values, most common ones are "Backend", "Frontend" and "Mobile" in case of IC roles. For management roles, it can be name of family or division. More on how to interpret and work with the normalized salaries can be found in the [compensation](compensation.md) guide.

| Career Track               | Min P | Max P | Grade | Job Title                                       | Min Salary | Next Salary |
|----------------------------|-------|-------|-------|-------------------------------------------------|------------|-------------|
| Product Division Lead      | 3.50  | 5.00  | L1    | VP Engineering, Product                         |     200000 |      300000 |
| Platform Division Lead     | 3.50  | 5.00  | L1    | VP Engineering, Platform                        |     200000 |      300000 |
| Product Family Lead        | 0.00  | 3.10  | M1    | Engineering Manager, {Discriminator}            |     120000 |      175000 |
| Product Family Lead        | 3.10  | 4.20  | D1    | Director of Engineering, {Discriminator}        |     175000 |      210000 |
| Product Family Lead        | 4.20  | 5.00  | D2    | Senior Director of Engineering, {Discriminator} |     210000 |      250000 |
| Platform Family Lead       | 0.00  | 3.10  | M1    | Engineering Manager, {Discriminator}            |     120000 |      175000 |
| Platform Family Lead       | 3.10  | 4.20  | D1    | Director of Engineering, {Discriminator}        |     175000 |      210000 |
| Platform Family Lead       | 4.20  | 5.00  | D2    | Senior Director of Engineering, {Discriminator} |     210000 |      250000 |
| Product Team Lead          | 0.00  | 1.40  | S1    | Engineering Manager                             |      69000 |       92000 |
| Product Team Lead          | 1.40  | 2.60  | S2    | Engineering Manager II                          |      92000 |      121000 |
| Product Team Lead          | 2.60  | 3.80  | M1    | Senior Engineering Manager                      |     121000 |      161000 |
| Product Team Lead          | 3.80  | 5.00  | M2    | Senior Engineering Manager II                   |     161000 |      207000 |
| Platform Team Lead         | 0.00  | 1.40  | S1    | Engineering Manager                             |      69000 |       92000 |
| Platform Team Lead         | 1.40  | 2.60  | S2    | Engineering Manager II                          |      92000 |      121000 |
| Platform Team Lead         | 2.60  | 3.80  | M1    | Senior Engineering Manager                      |     121000 |      161000 |
| Platform Team Lead         | 3.80  | 5.00  | M2    | Senior Engineering Manager II                   |     161000 |      207000 |
| Product Security Team Lead | 0.00  | 1.40  | S1    | Product Security Team Lead                      |      69000 |       92000 |
| Product Security Team Lead | 1.40  | 2.60  | S2    | Product Security Team Lead II                   |      92000 |      121000 |
| Product Security Team Lead | 2.60  | 3.80  | M1    | Snior Product Security Team Lead                |     121000 |      161000 |
| Product Security Team Lead | 3.80  | 5.00  | M2    | Senior Product Security Team Lead II            |     161000 |      207000 |
| Data Science Team Lead     | 0.00  | 1.40  | S1    | Team Lead, Data Science                         |      69000 |       92000 |
| Data Science Team Lead     | 1.40  | 2.60  | S2    | Team Lead II, Data Science                      |      92000 |      121000 |
| Data Science Team Lead     | 2.60  | 3.80  | M1    | Senior Team Lead, Data Science                  |     121000 |      161000 |
| Data Science Team Lead     | 3.80  | 5.00  | M2    | Senior Team Lead II, Data Science               |     161000 |      207000 |
| IT and Security Lead       | 0.00  | 1.40  | S1    | IT and Security Manager                         |      81000 |      115000 |
| IT and Security Lead       | 1.40  | 2.60  | S2    | IT and Security Manager II                      |     115000 |      150000 |
| IT and Security Lead       | 2.60  | 3.80  | M1    | Senior IT and Security Manager                  |     150000 |      184000 |
| IT and Security Lead       | 3.80  | 5.00  | M2    | Senior IT and Security Manager II               |     184000 |      230000 |
| Technical Leader           | 0.00  | 3.10  | S2    | Staff {Discriminator} Engineer                  |     115000 |      150000 |
| Technical Leader           | 3.10  | 4.20  | M1    | Senior Staff {Discriminator} Engineer           |     150000 |      184000 |
| Technical Leader           | 4.20  | 5.00  | D1    | Principal {Discriminator} Engineer              |     184000 |      230000 |
| Agile Coach                | 0.00  | 1.40  | IC2   | Agile Coach                                     |      69000 |       92000 |
| Agile Coach                | 1.40  | 2.60  | IC3   | Agile Coach II                                  |      92000 |      121000 |
| Agile Coach                | 2.60  | 3.80  | IC4   | Senior Agile Coach                              |     121000 |      161000 |
| Agile Coach                | 3.80  | 5.00  | IC5   | Senior Agile Coach II                           |     161000 |      207000 |
| Community Manager          | 0.00  | 1.40  | S1    | Community Manager                               |      46000 |       69000 |
| Community Manager          | 1.40  | 2.60  | S2    | Community Manager II                            |      69000 |       98000 |
| Community Manager          | 2.60  | 3.80  | M1    | Senior Community Manager                        |      98000 |      138000 |
| Community Manager          | 3.80  | 5.00  | M2    | Senior Community Manager II                     |     138000 |      184000 |
| Engineer                   | 0.00  | 1.20  | IC2   | {Discriminator} Engineer                        |      46000 |       69000 |
| Engineer                   | 1.20  | 2.40  | IC3   | {Discriminator} Engineer II                     |      69000 |       98000 |
| Engineer                   | 2.40  | 3.60  | IC4   | Senior {Discriminator} Engineer                 |      98000 |      138000 |
| Engineer                   | 3.60  | 5.00  | IC5   | Senior {Discriminator} Engineer II              |     138000 |      184000 |
| Product Security Engineer  | 0.00  | 1.20  | IC2   | Product Security Engineer                       |      46000 |       69000 |
| Product Security Engineer  | 1.20  | 2.40  | IC3   | Product Security Engineer II                    |      69000 |       98000 |
| Product Security Engineer  | 2.40  | 3.60  | IC4   | Senior Product Security Engineer                |      98000 |      138000 |
| Product Security Engineer  | 3.60  | 5.00  | IC5   | Senior Product Security Engineer II             |     138000 |      184000 |
| Data Scientist             | 0.00  | 1.20  | IC2   | Data Scientist                                  |      46000 |       69000 |
| Data Scientist             | 1.20  | 2.40  | IC3   | Data Scientist II                               |      69000 |       98000 |
| Data Scientist             | 2.40  | 3.60  | IC4   | Senior Data Scientist                           |      98000 |      138000 |
| Data Scientist             | 3.60  | 5.00  | IC5   | Senior Data Scientist II                        |     138000 |      184000 |
| IT Security Engineer       | 0.00  | 1.20  | IC2   | IT Security Engineer                            |      46000 |       69000 |
| IT Security Engineer       | 1.20  | 2.40  | IC3   | IT Security Engineer II                         |      69000 |       98000 |
| IT Security Engineer       | 2.40  | 3.60  | IC4   | Senior IT Security Engineer                     |      98000 |      138000 |
| IT Security Engineer       | 3.60  | 5.00  | IC5   | Senior IT Security Engineer II                  |     138000 |      184000 |
| Data Analyst               | 0.00  | 1.20  | IC2   | Data Analyst                                    |      40000 |       63000 |
| Data Analyst               | 1.20  | 2.40  | IC3   | Data Analyst II                                 |      63000 |       92000 |
| Data Analyst               | 2.40  | 3.60  | IC4   | Senior Data Analyst                             |      92000 |      127000 |
| Data Analyst               | 3.60  | 5.00  | IC5   | Senior Data Analyst II                          |     127000 |      161000 |
| IT Infrastructure Engineer | 0.00  | 1.20  | IC2   | IT Infrastructure Engineer                      |      40000 |       63000 |
| IT Infrastructure Engineer | 1.20  | 2.40  | IC3   | IT Infrastructure Engineer II                   |      63000 |       92000 |
| IT Infrastructure Engineer | 2.40  | 3.60  | IC4   | Senior IT Infrastructure Engineer               |      92000 |      127000 |
| IT Infrastructure Engineer | 3.60  | 5.00  | IC5   | Senior IT Infrastructure Engineer II            |     127000 |      161000 |
| QA Engineer                | 0.00  | 1.20  | IC1   | QA Engineer                                     |      35000 |       46000 |
| QA Engineer                | 1.20  | 2.40  | IC2   | QA Engineer II                                  |      46000 |       63000 |
| QA Engineer                | 2.40  | 3.60  | IC3   | Senior QA Engineer                              |      63000 |       92000 |
| QA Engineer                | 3.60  | 5.00  | IC4   | Senior QA Engineer II                           |      92000 |      127000 |
| IT Specialist              | 0.00  | 1.20  | IC1   | IT Specialist                                   |      35000 |       46000 |
| IT Specialist              | 1.20  | 2.40  | IC2   | IT Specialist II                                |      46000 |       63000 |
| IT Specialist              | 2.40  | 3.60  | IC3   | Senior IT Specialist                            |      63000 |       92000 |
| IT Specialist              | 3.60  | 5.00  | IC4   | Senior IT Specialist II                         |      92000 |      127000 |
| Community Coordinator      | 0.00  | 1.20  | IC1   | Community Coordinator                           |      35000 |       46000 |
| Community Coordinator      | 1.20  | 2.40  | IC2   | Community Coordinator II                        |      46000 |       63000 |
| Community Coordinator      | 2.40  | 3.60  | IC3   | Senior Community Coordinator                    |      63000 |       92000 |
| Community Coordinator      | 3.60  | 5.00  | IC4   | Senior Community Coordinator II                 |      92000 |      127000 |
